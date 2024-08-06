# Sudoku_Game

## Objective: 
  - The Sudoku game is a number puzzle where the goal is to fill a 9x9 grid with digits so that each column, each row, and each of the nine 3x3 subgrids contain all of the       digits from 1 to 9. This implementation uses the backtracking algorithm to solve Sudoku puzzles.

## Key Features:
1. **Grid Representation:**

     - The Sudoku grid is represented using a 2D array int grid[9][9].
     - Each cell in the array can hold an integer from 1 to 9 or a 0 if the cell is empty.
2. **Backtracking Algorithm:**

      - The backtracking algorithm is used to solve the puzzle by attempting to fill cells with digits from 1 to 9.
      - If a digit fits without violating Sudoku rules, the algorithm proceeds to the next cell.
      - If no valid digit is found for a cell, the algorithm backtracks to the previous cell and tries the next possible digit.
3. **Validation:**

      - Functions are used to check if placing a digit in a cell is valid according to Sudoku rules:
      - Row Check: Ensures the digit is not repeated in the current row.
      - Column Check: Ensures the digit is not repeated in the current column.
      - Subgrid Check: Ensures the digit is not repeated in the current 3x3 subgrid.
4. **User Interface:**

    - The grid can be input by the user or read from a predefined setup.
    - The solved Sudoku grid is displayed on the console.

## Implementation Details:
1. **Grid Initialization:**

    - The grid is initialized with a predefined puzzle or taken as input from the user.
2. **Solving the Puzzle:**

    - The solveSudoku() function implements the backtracking algorithm.
    - It uses the findEmptyLocation() function to locate the next empty cell.
    - The isSafe() function checks if placing a digit in a cell is valid.
3. **Printing the Grid:**

    - The printGrid() function prints the current state of the grid.
