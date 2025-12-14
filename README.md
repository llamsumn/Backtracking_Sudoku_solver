# GRADED ASSIGNMENT: Sudoku Puzzle Solver Agent

## Overview

This repository contains the complete implementation of a Sudoku Puzzle Solver Agent, developed as a graded assignment. The project addresses the Sudoku challenge as a classic **Constraint Satisfaction Problem (CSP)**, where the goal is to efficiently solve the 9x9 grid.

To achieve optimal computational performance and correctness, the solver implements a **Backtracking search algorithm synergized with the Minimum Remaining Values (MRV) Heuristic**. This combined approach applies a "fail-first" strategy to aggressively prune the search space, significantly improving speed and efficiency compared to naive backtracking.

## Project: Sudoku Puzzle Solver Agent

### Summary
The core of this project is a Python-based agent designed to read an unsolved 9x9 Sudoku grid and determine the single, correct solution by satisfying all constraints. The entire solving process is encapsulated within an **Object-Oriented Programming (OOP)** structure, storing the grid state and managing the main solving flow within a dedicated class.

### Key Features Implemented

1.  **Minimum Remaining Values (MRV) Heuristic:** The solver prioritizes the unassigned cell (variable) that has the *fewest* possible valid numbers (domains) remaining. This "fail-first" approach ensures that dead-end paths are identified and terminated early.
2.  **Backtracking Search:** The fundamental recursive search algorithm that systematically tries to assign values to variables, undoing the assignment (backtracking) when a conflict is detected .
3.  **Initial Validation:** The implementation begins with a validation step to filter out unsolvable or invalid puzzle arrays before starting the complex search process, which enhances overall robustness.
4.  **Constraint Checking (Row, Column, Box):** Robust functions ensure a proposed number placement satisfies all three core Sudoku rules: uniqueness across the row, uniqueness across the column, and uniqueness within the 3x3 block.
5.  **Efficient Grid Representation:** The 9x9 grid is efficiently handled using Python's 2D list/array data structures, allowing for fast state manipulation and constraint lookups.

## Technologies Used

* **Language:** Python
* **Environment:** Jupyter Notebook `.ipynb`
* **Concepts:** Constraint Satisfaction Problems (CSP), Search Algorithms (Backtracking), Minimum Remaining Values (MRV) Heuristic, Object-Oriented Programming (OOP), Recursion, 2D Array/List Structures.

## How to Run the Code

This project is contained within a single Jupyter Notebook file (`sudoku.ipynb`). The PDF report (`report.pdf`) provides a theoretical background on the chosen methodology.

1.  **Prerequisites:** Ensure you have **Python 3** installed on your system.
2.  **Environment:** The code is designed to run in a Jupyter environment (Jupyter Notebook or JupyterLab). You can install it via pip:
    ```bash
    pip install jupyter
    ```
3.  **Run:** Launch the notebook interface from your terminal:
    ```bash
    jupyter notebook
    ```
4.  **Execute:** Open the `sudoku.ipynb` file in your browser. The notebook defines the solver class and demonstrates its operation on sample puzzles. Run the cells sequentially to execute the solver agent.

## Contact

| Component | Information |
| :--- | :--- |
| **Author** | Lam Chun Lung Leo |
| **Email** | leolam725@gmail.com |
| **LinkedIn** | https://www.linkedin.com/in/lam-chun-lung-leo-leo-b27406172/ |
