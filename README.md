import random

def game():
    number_to_guess = random.randint(1, 10)
    guess = int(input("Guess a number between 1 and 10: "))

    while guess != number_to_guess:
        if guess < number_to_guess:
            print("Too low!")
        else:
            print("Too high!")
        guess = int(input("Guess again: "))

    print("Congratulations! You guessed the number.")

game()
