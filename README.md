I have implemented a class named “Board” that represents the 8-puzzle board, and I have implemented DFS and BFS methods in the driver class.


1) class Board:

DATA:

- A 2d array representing the board.

BEHAVIOR:

- A constructor for the 2d array.
- Method isGoal() that returns “true” if the board is the goal board and “false” otherwise.
- Method neighbors() that returns a queue with the neighbors of the board (i.e. all the boards that can be generated from moving the “0” cell in all directions).
- Method exch(int[][] board, int row, int col, int newRow, int newCol) that exchanges the positions of two cells.
- Method toString() that displays the 2d array as a 3x3 board.
- Method isSolvable() that returns “true” if the the goal board can be reached from this board and “false” otherwise.
- Method equals(Board state) that returns “true” if the parameter board is equal to this board and “false” otherwise.


2) method BFS:

I have implemented the pseudo code in the lecture’s slides as Java code, made the suitable modifications in order to apply the search on an instance of the class “Board”, added the variable “pathCost” in order to calculate the path cost, and added the method isSolvable() directly before the process of adding the neighbors of the current board to the frontier in order to avoid an infinite loop.


3) method DFS:

Exactly the same as the method of the BFS, but with the frontier as a “stack” instead of a “queue”.


Thank you :)
