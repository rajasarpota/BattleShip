I created the game of Battleship. I chose this because I enjoy creating and playing games, also I couldn’t think of another project to complete. This program first creates a “board”, which is just a list of a 5X5 array. It then selects a “battleship” which are variables randomly assigned to a certain row and column in the board. The player then has five turns to guess where the randomly selected battleship was placed by inputting the row and column spanning from 0-4. The algorithm required for this project to run includes:

 

1. Importing random and turtle 

2. The PrintBoard function that outputs the game board after every iteration (or turn)

3. The RandomRow function that returns a random integer between 0 to the length of the board

4. The RandomCol function that returns a random integer between 0 to the length of the board

5. The TurtleWinner and TurtleLoser functions serve only to display a message to the player whether or not they won the game. Honestly these functions really have no true purpose to the game, they were just implemented in order to fulfill the code length requirement.

6. The main function:

   a.  First creates the board as a list

   b.  Appends “0” throughout the entire board using a for loop, this is to display unpicked spots for the user to choose

   c.  The variables ShipRow and ShipCol are assigned to a random spot on the board using the RandomRow and RandomCol functions respectively

   d.  A counter for loop is made to track the number of iterations (or turns)

   ​	    i.   This is where the variables GuessRow and GuessCol are assigned by the user’s input

   ​       ii.   Then an if loop is used to determine if the user’s rows/column variables match the ship’s randomly assigned rows/columns.

   ​       iii.   If so, the game is over and the user wins and is greeted with a message as well as a turtle graphic.

   ​       iv.   If not, the else determines whether the number of turns exceeds 5 which results in game over, whether if the numbers inputted are valid/on the board, or if the numbers were already inputted. If the spot chosen isn’t where the ship is located, the board is updated with an X in the spot chosen using the PrintBoard function and the turn is iterated by 1. If the user loses, the game ends and displays a turtle graphic.

7. Using a while True loop, the main function is called to play the game, once the game is over it will ask the user whether they want to play again. If so, the game and the turtle screen resets for the next game. 