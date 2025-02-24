# Sudoku Solver (Backtracking)

This project implements a Sudoku solver using the backtracking algorithm in Python. It provides a simple and efficient way to solve Sudoku puzzles.

## Features

* **Sudoku Solving:** Solves 9x9 Sudoku puzzles.
* **Backtracking Algorithm:** Employs a recursive backtracking approach to find solutions.
* **Clear Output:** Displays the solved Sudoku grid in a readable format.
* **Easy to Use:** Simple code structure for easy modification and integration.

## Prerequisites

* Python 3.x

## Installation

1.  **Clone the Repository:**

    ```bash
    git clone [https://github.com/Praveen880890/Sodoku_Solver.git](https://www.google.com/search?q=https://github.com/Praveen880890/Sodoku_Solver.git)
    cd Sodoku_Solver
    ```

2.  **No additional installation is needed.** The project utilizes only standard Python libraries.

## Usage

1.  **Modify the Sudoku Grid:**

    * Open the `sudoku_solver.py` file.
    * Modify the `grid` variable to represent the Sudoku puzzle you want to solve.
    * Use `0` to represent empty cells.
    * Example grid:

    ```python
    grid = [
        [3, 0, 6, 5, 0, 8, 4, 0, 0],
        [5, 2, 0, 0, 0, 0, 0, 0, 0],
        [0, 8, 7, 0, 0, 0, 0, 3, 1],
        [0, 0, 3, 0, 1, 0, 0, 8, 0],
        [9, 0, 0, 8, 6, 3, 0, 0, 5],
        [0, 5, 0, 0, 9, 0, 6, 0, 0],
        [1, 3, 0, 0, 0, 0, 2, 5, 0],
        [0, 0, 0, 0, 0, 0, 0, 7, 4],
        [0, 0, 5, 2, 0, 6, 3, 0, 0]
    ]
    ```

2.  **Run the Script:**

    ```bash
    python sudoku_solver.py
    ```

3.  **View the Solution:**

    * The solved Sudoku grid will be printed to the console.
    * If no solution exist, the program will state that.

## Code Explanation

* **`is_valid_move(grid, row, col, num)`:**
    * Checks if placing `num` at `grid[row][col]` is valid according to Sudoku rules.
    * Ensures `num` is not present in the same row, column, or 3x3 subgrid.
* **`solve(grid, row, col)`:**
    * Recursive function implementing the backtracking algorithm.
    * Base case: Grid is filled, return `True`.
    * Iterates through possible numbers for empty cells.
    * If a valid move is found, recursively calls `solve`.
    * Backtracks if no valid move exists.
* **Main Execution:**
    * Initializes the Sudoku grid.
    * Calls `solve` to solve the puzzle.
    * Prints the results.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## Author

* Praveen880890

## License

This project is open source.
