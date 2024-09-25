# Algorithm Selection Guide: DP, Backtracking, Divide and Conquer, and Greedy

This guide helps you understand how to decide whether to use **Dynamic Programming (DP)**, **Backtracking**, **Divide and Conquer**, or **Greedy Algorithms** based on problem characteristics.

## 1. Dynamic Programming (DP)

**Dynamic Programming** is useful when the problem can be broken down into **overlapping subproblems** with a **recurrence relation**. You store the results of subproblems to avoid redundant computations.

### Problem Characteristics for DP:
- **Optimal Substructure**: Solutions to subproblems can be combined to solve the larger problem.
- **Overlapping Subproblems**: Same subproblems are solved multiple times.
- **Decision Making**: You often need to optimize (minimize/maximize) something.

### Common DP Problems:
- Fibonacci Sequence
- Knapsack Problem
- Longest Common Subsequence (LCS)
- Coin Change Problem

### How to Recognize DP Problems:
- The problem asks for minimum/maximum or count solutions.
- The problem can be broken into subproblems that overlap.
- It involves making choices at each step (e.g., take or leave an item).

---

## 2. Backtracking

**Backtracking** is a **trial-and-error** algorithm. It incrementally builds a solution and abandons (backtracks) as soon as it determines that the current partial solution is invalid.

### Problem Characteristics for Backtracking:
- **Search Space Exploration**: Requires exploring different combinations or arrangements.
- **Recursive Search**: The solution can be constructed by recursively exploring possibilities.
- **Constraints to Satisfy**: Solutions are rejected if they violate constraints.

### Common Backtracking Problems:
- N-Queens Problem
- Sudoku Solver
- Permutations and Combinations
- Subset Sum Problem

### How to Recognize Backtracking Problems:
- The problem asks to find all valid solutions from multiple combinations.
- Constraints need to be met, and partial solutions are discarded if invalid.

---

## 3. Divide and Conquer

**Divide and Conquer** breaks the problem into smaller, independent subproblems, solves them separately, and then combines the results.

### Problem Characteristics for Divide and Conquer:
- **Problem Decomposition**: Can be broken down into smaller, independent subproblems.
- **Combine Subproblem Solutions**: Solutions to subproblems can be combined.
- **Recursion**: Naturally uses recursion to solve each subproblem.

### Common Divide and Conquer Problems:
- Merge Sort and Quick Sort
- Binary Search
- Matrix Multiplication
- Closest Pair of Points

### How to Recognize Divide and Conquer Problems:
- The problem can be split into smaller independent parts.
- Recursion can be applied, and subproblems can be solved separately.

---

## 4. Greedy Algorithms

**Greedy Algorithms** work by making the locally optimal choice at every step with the hope that this leads to the global optimum.

### Problem Characteristics for Greedy:
- **Locally Optimal Choice**: You can make a locally optimal decision at each step.
- **No Future Impact**: Each local choice doesn’t affect future decisions.
- **Optimal Substructure**: The problem must exhibit optimal substructure.

### Common Greedy Problems:
- Dijkstra’s Algorithm (Shortest Path)
- Kruskal’s and Prim’s Algorithms (Minimum Spanning Tree)
- Fractional Knapsack Problem
- Huffman Coding

### How to Recognize Greedy Problems:
- The problem asks for an optimal solution.
- At each step, a choice can be made that seems the best without reconsidering.

---

## 5. Exhaustive Search (Brute Force)

If the problem requires exploring **all possible combinations** without clear strategies to reduce the search space, **Brute Force** may be appropriate.

### Problem Characteristics for Exhaustive Search:
- **No Clear Optimization**: Can’t break down into subproblems or optimize.
- **All Combinations Need to Be Explored**: Every possible combination or permutation must be checked.

### Common Brute Force Problems:
- Generating all subsets or permutations.
- Game-tree or puzzle-solving without constraints.

---

## Summary of Choosing the Right Algorithm:


| **Algorithm**       | **Key Characteristics**                                                                                 | **How to Recognize**                                                                                         |
|---------------------|---------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|
| **Dynamic Programming (DP)** | Overlapping subproblems, optimal substructure, recursive subproblems with memoization or tabulation | The problem involves **finding the minimum/maximum** or **counting ways** with **overlapping subproblems**.  |
| **Backtracking**     | Recursive search, constraints, explore all possible solutions, and backtrack when a partial solution fails | The problem involves **exploring all configurations** and **backtracking** once an invalid solution is found. |
| **Divide and Conquer**| Independent subproblems, recursion, and combining results                                                | The problem can be **divided into independent subproblems** and solved recursively before combining results.  |
| **Greedy**           | Local optimization at each step, no backtracking, globally optimal                                        | The problem can be solved by making **locally optimal choices** that lead to a **globally optimal solution**. |
| **Exhaustive Search (Brute Force)** | Explore all possibilities, no optimization, no pruning                                      | The problem requires **exploring all possible configurations or solutions** without clear optimization rules.  |

---

## Questions to Ask Yourself:

1. **Does the problem have overlapping subproblems?** If yes, consider **DP**.
2. **Do I need to explore multiple possible solutions and discard invalid ones?** If yes, think about **Backtracking**.
3. **Can I break the problem down into independent subproblems?** If yes, use **Divide and Conquer**.
4. **Can I make a local, greedy choice that will lead to an optimal solution?** If yes, try a **Greedy Algorithm**.
5. **Do I need to explore all possibilities with no clear shortcuts?** Consider **Exhaustive Search** or **Brute Force**.

---

### Let me know if you need further clarification on any specific approach!
