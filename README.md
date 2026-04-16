♟️ N-Queens Problem (LeetCode 51)
📌 Problem Statement

The N-Queens puzzle requires placing n queens on an n × n chessboard such that:

No two queens attack each other
No two queens share the same:
Row
Column
Diagonal

👉 Return all distinct solutions.

🧠 Approach (Backtracking)

We solve this using recursion + backtracking:

Place queens row by row
For each position, check if it's safe
Use helper arrays to track:
Columns (col)
Main diagonal (diag1 → row + col)
Anti-diagonal (diag2 → row - col)

If safe:

Place queen 'Q'
Move to next row
Backtrack if needed
