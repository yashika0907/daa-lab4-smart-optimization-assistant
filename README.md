# Smart Optimization Assistant

A Streamlit application demonstrating three classic dynamic programming
algorithms: Longest Common Subsequence (LCS), 0/1 Knapsack, and Matrix Chain
Multiplication (MCM). Each module displays its result, dynamic programming
table, execution time, and peak traced memory. A final tab summarizes
theoretical complexity.

## Requirements

- Python 3.10 or newer
- pip

## Run locally

In PowerShell, from the project directory:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
python -m streamlit run app.py
```

If PowerShell blocks virtual environment activation, allow it for the current
terminal and activate again:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
.\.venv\Scripts\Activate.ps1
```

## Features

- **LCS:** Find a longest common subsequence and inspect its DP table.
- **0/1 Knapsack:** Choose items maximizing profit within a capacity.
- **Matrix Chain Multiplication:** Find the minimum scalar multiplication
  cost and optimal parenthesization.
- **Complexity Summary:** Compare theoretical time, space, and subproblem
  counts for each algorithm.

## Example inputs

- LCS sequences: `ABCBDAB` and `BDCABA`
- Knapsack weights: `2,3,4,5`; values: `3,4,5,6`; capacity: `5`
- MCM dimensions: `10,30,5,60`

Execution time and memory measurements depend on the input and machine.
