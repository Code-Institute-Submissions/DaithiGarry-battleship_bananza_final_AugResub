![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)
# **Battleship Bonanza.**

Battleship Bonanza is a single player Python terminal game.

User try to sink the battleships of the computer in only ten attempts. Each battle ship is only one square on a 6 row X 6 column board.

![image of differnet displays](/assets/images/main_image.png)

## How to play

Battleship Bonanza is based on the well know strategic combat game know as "Battleships". 

In this version, a single player will attempt to sink 5 battleships which the computer has placed randomly on a 6 X 6 square grid. A direct hit to a battleship is represented by an "S" on the grid, while a miss is represented by an "X". The player will have 10 attempts to sink the 5 battleships. Faliure to do so, within 10 attempts will result in the player losing the game.

## Features 

### Existing Features
- Random battleships are placed on the board by the computer
- The player will only know where the battleships are placed when/if they guess the correct location marked with an "S".

![image of direct hit S and miss X](/assets/images/direct_hit_and_miss_image.png).

- Maintains the numbers of guesses the player has left

![number of turns remaining](/assets/images/number_of_turns_remaining.png)

- Accepts user inputs
- Input validation and error-checking
    - A player in unable to guess the same location twice during the same game.
    - A Player can only guess within a define grid

![guessing errors](/assets/images/errors%20.png)

- Date in maintained in classes

### Future Features
- Computer versus player 
- multiple players
- ships larger than 1X1
- ships located both vertically and horizontally on the grid


### Data model

The data class model was used to create Battleship Bonanza using two main classes. The board is used to store the attribites of the board, i.e. the board size, row details and column details.
The battleship class was used to store the battleship random generation and number of battleships.
Finally the PlayGame class is used to enforce the game rules.

### Testing

The project has been manually tested via the following:
- The code has been run through the PEP8 linter and confirmed that the only no issues found where indentation and line length issues.

- Given invalid inputs: string where numbers are expected, locations outside of the grid and same location twice during the same game.

## Bugs
- The comments under the print_board definition on line 14 created an indentation error which i could only resolved by placing it above the def and not under the line.
- Before final deployment a new file was created to clean out indentation errors from the file when opening in Heroku app.
- A new set of images were created for the readme file as during the copy/paste to the file, a file name issue created a text overlap in the readme file which hid text from view. A new set of images were copy/pasted an now file is aligned correctly.
### Solved Bugs
App would not deploy due to indentation error. This was fixed by creating a new file.

### Remaining bugs
- No bugs remaining

## Validator Testing
- PEP8
  - No major errors were returned other than indentation, line length and spacing from PEP8online.com

## Deployment

This project was deployed to Heroku
This project was deployed to github

## Credit

Code was influenced by battleship games discussed on ArjanCodes and gbrough (knowledge mavens) youtube channels.