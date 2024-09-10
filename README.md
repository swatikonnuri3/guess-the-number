Description:

    Setup:
        The program starts by importing the random module to generate a random number.
        The number is selected within a predefined range (e.g., 1 to 100).

    Input from User:
        The user is prompted to guess the number.

    Feedback:
        After each guess, the program checks if the guessed number is too high, too low, or correct.
        If the guess is incorrect, the program provides a hint, such as "Too high!" or "Too low!" and prompts the user to guess again.

    Loop:
        The guessing continues in a loop until the user guesses the correct number.

    Win Condition:
        When the correct number is guessed, the program displays a congratulatory message and optionally reports how many attempts it took.

Example Code:

python

import random

def guess_number():
    number = random.randint(1, 100)
    attempts = 0
    print("I have chosen a number between 1 and 100. Can you guess it?")
    
    while True:
        guess = int(input("Enter your guess: "))
        attempts += 1
        
        if guess < number:
            print("Too low!")
        elif guess > number:
            print("Too high!")
        else:
            print(f"Congratulations! You've guessed the number {number} in {attempts} attempts.")
            break

guess_number()

Key Concepts:

    Random number generation: The random.randint() function generates a number within a specified range.
    Loops: The guessing continues until the user finds the correct number.
    Conditional statements: Used to give feedback on whether the guess is too high, too low, or correct.

This simple game demonstrates key programming concepts like loops, conditionals, and user input.
