import random

beg = 1
end = 100
answer = random.randint(beg, end)
attempts = 0

print("\n------------------------PYTHON GUESSING GAME------------------------\n")

while True:
    guess = input(
        "Guess a number between 1 and 100! (or q to quit): ").lower()
    if guess == "q":
        break

    if guess.isdigit():
        guess = int(guess)
        attempts += 1

        if guess < beg or guess > end:
            print("Type a number between 1 and 100!")

        elif guess < answer:
            print("Too low!")
        elif guess > answer:
            print("Too high!")

        else:
            print(
                f"\nCorrect, the number was {answer}!. It took you {attempts} attempts!\n")
            while True:
                play_again = input(
                    "Would you like to play again? (yes/no): ").lower()

                if play_again in ["yes", "y"]:
                    print("\nGreat!\n")
                    answer = random.randint(beg, end)
                    attempts = 0
                    break

                elif play_again in ["no", "n"]:
                    print("\nThank you for playing!\n")
                    exit()

                else:
                    print("\nplease type (yes/no)\n")

    else:
        print("\nInvalid guess!\n")
