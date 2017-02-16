# Guessing-Game
import random
my_number = random.randrange(101)

guessesTaken = 0
print("Hey, what's up? What should I call you?")
name = input('Name: ')
print('\nSup' , name + ', I am thinking of a number between 1 and 100')
while guessesTaken <6:
    my_guess = int(input('Take a guess: '))
    guessesTaken = guessesTaken +1
    if my_guess > my_number:
        print("Wrong you are too high")
    elif my_guess < my_number:
        print("Wrong you are too low")
    elif my_guess == my_number:
        print('You guessed it right,' +my_number + 'is correct')
        print("It took you", + guessesTaken + ", guesses to figure out the hidden number")
        break
