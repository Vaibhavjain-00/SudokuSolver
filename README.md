# 🧩 Sudoku Solver (Backtracking in Java)

A simple Java implementation of a **Sudoku Solver** using the **Backtracking algorithm**.
The program fills a 9×9 Sudoku board by trying valid numbers recursively until the puzzle is solved.

---

## 🚀 Features

* Solves standard **9×9 Sudoku puzzles**
* Uses **Backtracking + Recursion**
* Validates moves based on:

  * Row constraint
  * Column constraint
  * 3×3 subgrid constraint
* Prints solved board to console
* Handles unsolvable puzzles gracefully

---

## 🧠 Algorithm Overview

The solver works as follows:

1. Scan the board to find an empty cell (`0` represents empty).
2. Try placing numbers from **1 to 9**.
3. Check if the number is valid using:

   * Row check
   * Column check
   * Subgrid check
4. If valid → place number and continue recursively.
5. If dead end → **backtrack** and try next number.
6. If no empty cells remain → puzzle solved.

Time complexity is exponential in the worst case, but efficient for standard puzzles.

---

## 📂 Project Structure

```
com.kunal.backtracking
└── SudokuSolver.java
```

---

## ▶️ How to Run

### 1. Compile

```bash
javac com/kunal/backtracking/SudokuSolver.java
```

### 2. Run

```bash
java com.kunal.backtracking.SudokuSolver
```

---

## 🧪 Example Input Board

```
3 0 6 5 0 8 4 0 0
5 2 0 0 0 0 0 0 0
0 8 7 0 0 0 0 3 1
0 0 3 0 1 0 0 8 0
9 0 0 8 6 3 0 0 5
0 5 0 0 9 0 6 0 0
1 3 0 0 0 0 2 5 0
0 0 0 0 0 0 0 7 4
0 0 5 2 0 6 3 0 0
```

`0` represents an empty cell.

---

## 📤 Example Output

```
3 1 6 5 7 8 4 9 2
5 2 9 1 3 4 7 6 8
4 8 7 6 2 9 5 3 1
2 6 3 4 1 5 9 8 7
9 7 4 8 6 3 1 2 5
8 5 1 7 9 2 6 4 3
1 3 8 9 4 7 2 5 6
6 9 2 3 5 1 8 7 4
7 4 5 2 8 6 3 1 9
```

---

## 🔧 Customizing the Puzzle

Modify the `board` array in `main()`:

```java
int[][] board = new int[][]{
    { ... },
    { ... }
};
```

Use `0` for empty cells.

---

## 📚 Concepts Used

* Recursion
* Backtracking
* 2D Arrays
* Constraint Validation
* Problem Solving

---


