# Number-Guessing-Game
A simple Python-based ‘Guess the Number' game that uses random number generation and user input handling with error management.
import random

guess_the_number = random.randint(1, 100)

while True:
    try:
        guess = int(input('Guess the number b/w 1 to 100: '))
        if guess < guess_the_number:
            print('Too Low')
        elif guess > guess_the_number:
            print('Too High')
        else:
            print('Congratulation You guessed the number.')
            break
    except ValueError:
        print('Please enter a valid number')
