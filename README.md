This program is a simple implementation of the classic Tic-Tac-Toe game in C++. Two players can play the game alternately, and the program checks for a winner or a draw after each move.

Code Breakdown
displayBoard Function:

Prints the current state of the 3x3 game board.
Uses a grid-like format with rows and columns separated by | and --------- for visual clarity.
Called after every move to update the board view.
Example Output:

markdown
Copy code
 X | O |  
---------
   | X |  
---------
   |   | O
checkWin Function:

Checks if the current player has won the game.
Evaluates the rows, columns, and both diagonals for a winning condition (all elements match the current player's symbol).
Returns true if a win is detected; otherwise, false.
checkDraw Function:

Checks if all cells on the board are filled and no winner is present.
Returns true if the board is full and there's no winner, indicating a draw.
playGame Function:

Core gameplay logic.
Initializes an empty 3x3 board with spaces (' ').
Alternates turns between Player 'X' and Player 'O'.
Prompts the current player to enter their move (row and column).
Validates the move to ensure the selected cell is empty and within bounds.
Updates the board with the player's symbol (X or O).
Checks for a win or draw after each move:
If a player wins, it announces the winner and ends the game.
If the game ends in a draw, it displays a message and ends the game.
Asks players if they want to play again, recursively restarting the game if they agree.
main Function:

Simply calls playGame() to start the game.
Features
Player Turn Management:
Alternates between players 'X' and 'O'.
Move Validation:
Ensures moves are within bounds and cells are not already occupied.
Win and Draw Detection:
Determines the game outcome based on board state after each move.
Replay Option:
Allows players to restart the game after it ends.
