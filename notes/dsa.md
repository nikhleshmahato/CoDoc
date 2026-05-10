# Data Structures and Algorithms (DSA) – Complete Notes

# Table of Contents

1. Introduction to DSA
2. Time and Space Complexity
3. Arrays
4. Strings
5. Linked List
6. Stack
7. Queue
8. Hashing
9. Recursion
10. Searching Algorithms
11. Sorting Algorithms
12. Trees
13. Binary Search Tree
14. Heap
15. Trie
16. Graphs
17. Greedy Algorithms
18. Dynamic Programming
19. Backtracking
20. Bit Manipulation
21. Sliding Window
22. Two Pointer Technique
23. Prefix Sum
24. Segment Tree
25. Disjoint Set Union
26. Important Algorithms
27. DSA Interview Preparation Strategy
28. Practice Platforms

---

# 1. Introduction to DSA

## What is DSA?

DSA stands for:

* Data Structures
* Algorithms

### Data Structure

A way to organize and store data efficiently.

Examples:

* Array
* Linked List
* Stack
* Queue
* Tree
* Graph

### Algorithm

A step-by-step procedure to solve a problem.

Examples:

* Binary Search
* Merge Sort
* Dijkstra Algorithm

---

## Why Learn DSA?

* Improves problem-solving skills
* Helps write optimized code
* Important for coding interviews
* Required in software engineering
* Used in AI, ML, Web, Systems, Games, Databases

---

# 2. Time and Space Complexity

## Time Complexity

Measures how execution time increases with input size.

### Big O Notation

| Complexity | Name         |
| ---------- | ------------ |
| O(1)       | Constant     |
| O(log n)   | Logarithmic  |
| O(n)       | Linear       |
| O(n log n) | Linearithmic |
| O(n²)      | Quadratic    |
| O(2^n)     | Exponential  |
| O(n!)      | Factorial    |

---

## Space Complexity

Measures memory usage.

### Example

```python
arr = [1,2,3]
```

Space Complexity = O(n)

---

## Complexity Comparison

| Best     | Acceptable | Bad    |
| -------- | ---------- | ------ |
| O(1)     | O(n log n) | O(n²)  |
| O(log n) | O(n)       | O(2^n) |

---

# 3. Arrays

## Definition

Collection of elements stored in contiguous memory.

```python
arr = [1,2,3,4]
```

---

## Operations

| Operation     | Complexity |
| ------------- | ---------- |
| Access        | O(1)       |
| Search        | O(n)       |
| Insert End    | O(1)       |
| Insert Middle | O(n)       |
| Delete        | O(n)       |

---

## Advantages

* Fast indexing
* Cache friendly

## Disadvantages

* Fixed size
* Costly insertion/deletion

---

## Important Concepts

### Traversal

```python
for i in arr:
    print(i)
```

### Prefix Sum

```python
prefix[i] = prefix[i-1] + arr[i]
```

### Kadane's Algorithm

Used for maximum subarray sum.

Complexity: O(n)

---

# 4. Strings

## Definition

Sequence of characters.

```python
s = "hello"
```

---

## Important Operations

| Operation     | Complexity |
| ------------- | ---------- |
| Access        | O(1)       |
| Concatenation | O(n)       |
| Search        | O(n)       |

---

## Important Algorithms

### Pattern Matching

* Naive Algorithm
* KMP Algorithm
* Rabin-Karp
* Z Algorithm

---

## Palindrome Check

```python
s == s[::-1]
```

---

# 5. Linked List

## Definition

Linear data structure where elements are connected using pointers.

---

## Types

### Singly Linked List

```text
10 -> 20 -> 30 -> NULL
```

### Doubly Linked List

```text
NULL <- 10 <-> 20 <-> 30 -> NULL
```

### Circular Linked List

Last node points to first node.

---

## Operations

| Operation        | Complexity |
| ---------------- | ---------- |
| Insert Beginning | O(1)       |
| Insert End       | O(n)       |
| Delete           | O(n)       |
| Search           | O(n)       |

---

## Advantages

* Dynamic size
* Easy insertion/deletion

## Disadvantages

* Extra memory for pointers
* Slow access

---

# 6. Stack

## Definition

LIFO (Last In First Out)

---

## Operations

| Operation | Complexity |
| --------- | ---------- |
| Push      | O(1)       |
| Pop       | O(1)       |
| Peek      | O(1)       |

---

## Applications

* Function calls
* Undo operations
* Expression evaluation
* Backtracking

---

## Example

```python
stack = []
stack.append(10)
stack.pop()
```

---

# 7. Queue

## Definition

FIFO (First In First Out)

---

## Types

* Simple Queue
* Circular Queue
* Priority Queue
* Deque

---

## Operations

| Operation | Complexity |
| --------- | ---------- |
| Enqueue   | O(1)       |
| Dequeue   | O(1)       |

---

## Applications

* CPU scheduling
* BFS traversal
* Buffer management

---

# 8. Hashing

## Definition

Technique to map keys to values.

---

## Hash Table

Stores:

```python
{
  "name": "Nik"
}
```

---

## Complexity

| Operation | Average |
| --------- | ------- |
| Insert    | O(1)    |
| Delete    | O(1)    |
| Search    | O(1)    |

---

## Collision Handling

### Chaining

Use linked lists.

### Open Addressing

* Linear probing
* Quadratic probing
* Double hashing

---

# 9. Recursion

## Definition

Function calling itself.

---

## Structure

```python

def solve(n):
    if n == 0:
        return

    solve(n-1)
```

---

## Important Concepts

* Base case
* Recursive case
* Stack memory

---

## Applications

* Tree traversal
* Backtracking
* Divide and conquer

---

# 10. Searching Algorithms

# Linear Search

## Complexity

O(n)

```python
for i in arr:
    if i == target:
        return True
```

---

# Binary Search

Works on sorted arrays.

## Complexity

O(log n)

```python
low = 0
high = len(arr)-1
```

---

## Binary Search Pattern

* Search space reduction
* Mid calculation
* Monotonic condition

---

# 11. Sorting Algorithms

# Bubble Sort

## Complexity

O(n²)

---

# Selection Sort

## Complexity

O(n²)

---

# Insertion Sort

## Complexity

O(n²)

---

# Merge Sort

## Divide and Conquer

## Complexity

O(n log n)

---

# Quick Sort

## Complexity

Average: O(n log n)
Worst: O(n²)

---

# Heap Sort

## Complexity

O(n log n)

---

## Stable vs Unstable Sorting

| Stable      | Unstable   |
| ----------- | ---------- |
| Merge Sort  | Quick Sort |
| Bubble Sort | Heap Sort  |

---

# 12. Trees

## Definition

Hierarchical data structure.

---

## Terminology

* Root
* Parent
* Child
* Leaf
* Height
* Depth

---

## Binary Tree

Each node has at most 2 children.

---

## Traversals

### DFS

* Inorder
* Preorder
* Postorder

### BFS

* Level Order Traversal

---

## Complexity

Traversal = O(n)

---

# 13. Binary Search Tree (BST)

## Property

Left subtree < Root < Right subtree

---

## Complexity

| Operation | Average  |
| --------- | -------- |
| Insert    | O(log n) |
| Search    | O(log n) |
| Delete    | O(log n) |

Worst Case = O(n)

---

## Applications

* Searching
* Ordered data
* Databases

---

# 14. Heap

## Definition

Complete binary tree.

---

## Types

### Max Heap

Parent > Child

### Min Heap

Parent < Child

---

## Priority Queue

Implemented using heap.

---

## Complexity

| Operation | Complexity |
| --------- | ---------- |
| Insert    | O(log n)   |
| Delete    | O(log n)   |
| Peek      | O(1)       |

---

# 15. Trie

## Definition

Tree used for string searching.

---

## Applications

* Autocomplete
* Dictionary
* Spell checker

---

## Complexity

Search = O(length of word)

---

# 16. Graphs

## Definition

Collection of nodes and edges.

---

## Types

* Directed Graph
* Undirected Graph
* Weighted Graph
* Cyclic Graph
* Acyclic Graph

---

## Representation

### Adjacency Matrix

### Adjacency List

---

# Graph Traversal

## BFS

Uses queue.

Complexity: O(V + E)

---

## DFS

Uses stack/recursion.

Complexity: O(V + E)

---

# Shortest Path Algorithms

## Dijkstra Algorithm

Works for positive weights.

Complexity: O(E log V)

---

## Bellman Ford

Handles negative weights.

---

## Floyd Warshall

All-pairs shortest path.

---

# Minimum Spanning Tree

## Kruskal Algorithm

Uses DSU.

## Prim Algorithm

Uses priority queue.

---

# 17. Greedy Algorithms

## Definition

Choose locally optimal solution.

---

## Examples

* Activity Selection
* Huffman Coding
* Fractional Knapsack
* Job Sequencing

---

## When Greedy Works

* Greedy choice property
* Optimal substructure

---

# 18. Dynamic Programming

## Definition

Optimization using overlapping subproblems.

---

## Concepts

* Memoization
* Tabulation

---

## Famous Problems

### Fibonacci

### 0/1 Knapsack

### Longest Common Subsequence

### Matrix Chain Multiplication

### Longest Increasing Subsequence

---

## DP Steps

1. Define state
2. Find recurrence
3. Base case
4. Memoize/tabulate

---

# 19. Backtracking

## Definition

Try all possibilities and backtrack.

---

## Applications

* N Queens
* Sudoku Solver
* Rat in Maze
* Permutations

---

## Complexity

Usually exponential.

---

# 20. Bit Manipulation

## Operators

| Operator | Meaning     |    |
| -------- | ----------- | -- |
| &        | AND         |    |
|          |             | OR |
| ^        | XOR         |    |
| ~        | NOT         |    |
| <<       | Left Shift  |    |
| >>       | Right Shift |    |

---

## Important Tricks

### Check Odd/Even

```python
n & 1
```

### Swap Numbers

Using XOR.

### Count Set Bits

Brian Kernighan Algorithm.

---

# 21. Sliding Window

## Definition

Technique for subarrays/substrings.

---

## Applications

* Maximum sum subarray
* Longest substring
* Fixed-size window problems

---

## Complexity

Usually O(n)

---

# 22. Two Pointer Technique

## Definition

Use two indices for optimization.

---

## Applications

* Sorted array problems
* Pair sum
* Remove duplicates

---

# 23. Prefix Sum

## Definition

Precompute cumulative sums.

---

## Formula

```python
prefix[i] = prefix[i-1] + arr[i]
```

---

## Applications

* Range sum query
* Subarray problems

---

# 24. Segment Tree

## Definition

Tree for range queries.

---

## Applications

* Range sum
* Range minimum
* Updates

---

## Complexity

| Operation | Complexity |
| --------- | ---------- |
| Build     | O(n)       |
| Query     | O(log n)   |
| Update    | O(log n)   |

---

# 25. Disjoint Set Union (DSU)

## Definition

Tracks connected components.

---

## Operations

### Find

### Union

---

## Optimizations

* Path compression
* Union by rank

---

## Applications

* Kruskal Algorithm
* Network connectivity

---

# 26. Important Algorithms

# Divide and Conquer

* Merge Sort
* Quick Sort
* Binary Search

---

# Graph Algorithms

* BFS
* DFS
* Dijkstra
* Bellman Ford
* Floyd Warshall
* Topological Sort

---

# String Algorithms

* KMP
* Rabin Karp
* Z Algorithm
* Trie

---

# Advanced Algorithms

* Fenwick Tree
* Sparse Table
* Mo's Algorithm
* Heavy Light Decomposition
* Suffix Array

---

# 27. DSA Interview Preparation Strategy

# Beginner Stage

Learn:

* Arrays
* Strings
* Linked List
* Stack
* Queue
* Recursion

Practice Easy Problems.

---

# Intermediate Stage

Learn:

* Trees
* BST
* Heap
* Hashing
* Binary Search
* Sliding Window

Practice Medium Problems.

---

# Advanced Stage

Learn:

* Graphs
* DP
* Segment Tree
* Trie
* Advanced Algorithms

Practice Hard Problems.

---

# Problem Solving Tips

* Understand brute force first
* Optimize gradually
* Learn patterns
* Revise frequently
* Solve daily

---

# 28. Practice Platforms

## Coding Practice

* LeetCode
* Codeforces
* CodeChef
* HackerRank
* GeeksforGeeks
* AtCoder

---

# Important DSA Patterns

| Pattern         | Usage              |
| --------------- | ------------------ |
| Sliding Window  | Subarrays          |
| Two Pointer     | Sorted arrays      |
| Binary Search   | Monotonic problems |
| DP              | Optimization       |
| Greedy          | Local optimum      |
| Backtracking    | Combinations       |
| Graph Traversal | Connectivity       |

---

# Common Interview Questions

## Arrays

* Two Sum
* Maximum Subarray
* Merge Intervals

## Linked List

* Reverse Linked List
* Detect Cycle

## Trees

* Lowest Common Ancestor
* Diameter of Tree

## Graph

* Number of Islands
* Shortest Path

## Dynamic Programming

* Coin Change
* House Robber
* Knapsack

---

# Competitive Programming Topics

* Number Theory
* Combinatorics
* Modular Arithmetic
* Fast Exponentiation
* Sieve of Eratosthenes
* Bitmask DP

---

# Real World Applications of DSA

| Topic   | Real Use        |
| ------- | --------------- |
| Graphs  | Google Maps     |
| Trie    | Search Engine   |
| Heap    | OS Scheduling   |
| Hashing | Databases       |
| DP      | AI Optimization |
| Queue   | Task Scheduling |

---

# Recommended Learning Order

1. Complexity Analysis
2. Arrays
3. Strings
4. Linked List
5. Stack
6. Queue
7. Hashing
8. Recursion
9. Sorting
10. Searching
11. Trees
12. Heap
13. Graphs
14. Greedy
15. Dynamic Programming
16. Segment Tree
17. Advanced Algorithms

---

# Final Advice

* Consistency is more important than speed.
* Focus on patterns, not memorization.
* Build logic through problem solving.
* Revise old problems regularly.
* Write clean and optimized code.

---

# End of Notes
