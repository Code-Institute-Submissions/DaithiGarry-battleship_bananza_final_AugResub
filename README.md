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


![position already guessed](/assets/images/position%20already%20guessed.png)


    - A Player can only guess within a define grid row/column

Row - the image below shows the row 9 being selected, which is outside the grid range of 1-6.

![row position not on grid](/assets/images/row%20position%20not%20on%20the%20board.png)

Column - the image below shows the column u being selected, which is outside the grid range of A-F. 

![column position not on grid](/assets/images/column%20position%20not%20on%20the%20board.png)

    - A player cannot enter a blank space for row or column position

Row - blank input entry for row selection shows program does not crash 

![blank entry for row position](/assets/images/blank%20input%20for%20battlesip%20board%20row%20selection.png)


Column - blank input entry for column selection shows program does not crash 

![Blank entry for column position](/assets/images/blank%20input%20for%20battlesip%20board%20column%20selection.png)



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
The user blank input issue has been resolved via adding "" to the list of unacceptable inputs by the user as seen below, highlighted in yellow.
![user blank space input bug fix](/assets/images/bug%20fix%20for%20blank%20space.png)
### Remaining bugs
- No bugs remaining

## Validator Testing
- PEP8
  - No major errors were returned other than line length PEP8online.com
  ![PEP8 online results](/assets/images/PEP8%20online%20results.png)

## Deployment

This project was deployed to Heroku originally. The new update has been manualy deployed since the recent updates on the 21AUG2022
This project was deployed to github

## Credit

Code was influenced by battleship games discussed on ArjanCodes and gbrough (knowledge mavens) youtube channels.