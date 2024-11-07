# Sudoku Classic v1

**Purpose**: To create a Sudoku classic game with basic functionality and minimal technologies.

## About Sudoku

- The puzzle is a 9 x 9 grid with a total of 81 cells.
- There are 9 rows, 9 columns, and 9 blocks (3 x 3 grids).
- Rows are counted top to bottom from 1 to 9. Columns are counted left to right from 1 to 9. Blocks are counted left to right then top down from 1 to 9.
- When a puzzle is loaded with values, those starting values are called givens. The cells that are empty are called guesses.
- The puzzle is complete when the digits 1 to 9 are placed in all cells where no row, column, or block has duplicate digits.

## Conceptual Flow

1. **Start (Web Page Loads)**
   - Load Sudoku Puzzle that contains the puzzle for user to solve.
     - Note: Puzzle cells are not editable. The empty cells are editable by the user. There will be design distinction for editable and uneditable cells.
2. **User Actions**
   - Possible Actions
     - Enter/Edit Numbers in editable cells.
     - Click "Reset Board"
       - This action reloads the puzzle for the user to solve.
       - This action clears the user's entered values.
     - Click "Submit Solution"
       - Initiates **Solution Validation**
3. **Solution Validation**
   - Checks each cell against the solution.
     - If an empty cell is found, display a message "Incomplete solution." and stop checking. Back to **User Actions** flow.
     - If a cell doesn't match the solution, display message "Sorry, incorrect solution." and stop checking. Back to **User Actions** flow.
     - If no mismatch is found after checking all the cells against the solution, display message "Congratulations! You solved the puzzle." and **END**.

## Technologies To Use

- HTML/CSS/JavaScript
- Source Control: Git/GitHub
- Project Management: Jira

## Project Structure

```bash
├── index.html
├── css
│   ├── reset.css
│   └── styles.css
├── js/
│   └── main.js
├── assets
│   ├── fonts
│   ├── icons
│   └── images
├── tests
└── README.md
```
