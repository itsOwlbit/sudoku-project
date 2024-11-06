# Sudoku Classic v1

**Purpose**: To create a Sudoku classic game with basic functionality and minimal technologies.

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
- CI/CD: GitHub Actions
- Testing: Jest or Mocha?

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
