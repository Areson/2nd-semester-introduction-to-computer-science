# Lab 3.04 - Guess My Number

## Create a Guessing Game using Loops
We are going to create a guessing game where the player tries to guess a number between 1 and 10 that the computer picked. To help you out, we’ve made some functions for you to use:
 
```python
import nccs

# Gets a guess from the player, between 1 and 10, and returns that guess.
nccs.getPlayerGuess()

# Asks the player if they want to play again. Returns True if they answered “yes” and False if they
# answered “no”.
nccs.askPlayAgain()
```

Feel free to use these in your program.

## Version 1
#### Requirements
* The computer should pick a number between 1 and 10
  * Remember `random` and `randint`
* The player should pick a number between 1 and 10
* The program should tell the player if they guessed correctly or not
* Once the game has been played, the program should ask the player if they want to play again. If the play answers "yes" then repeat the game.

*Remember*: We have the helper functions you can use for your game.

## Version 2
In this version the player gets 3 chances to guess the number. Once they run out of guesses the game is over!
* After each guess the program will tell the player if they were correct or not
  * If the player is correct the program will tell them they one and the game will end
  * If the player is wrong the program will tell them and the player will have one less chance
* If the player runs out of chances without guessing the number the program should tell them they lost and the game should end

## Bonus
As a bonus, take version 2 of the game and enhance it (put this version in `bonus.py`). In addition to the requirements for version 2, add these:
* Once the game has ended ask the player if they want to play again. If they do, start a new game.
* Write your own function with this contract:
  ```python
  howFarOff(guess, number)
  ```
  This function should take the player's guess and the computer's number and print out if the player's guess was higher or lower than the computer's number.
* After each _wrong_ guess call `howFarOff` to give the player a hint