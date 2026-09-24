practical-1
summary:
Sorting algorithms are methods used to arrange data in a specific order, usually ascending or descending. Common sorting algorithms include:

Bubble Sort: Repeatedly compares adjacent elements and swaps them if they are in the wrong order. Simple but inefficient for large datasets.
Selection Sort: Finds the smallest element and places it in its correct position. It is easy to understand but generally slow.
Insertion Sort: Builds the sorted list one element at a time. It works well for small or nearly sorted datasets.
Merge Sort: Divides the data into smaller parts, sorts them, and merges them. It has good performance and a time complexity of O(n log n).
Quick Sort: Selects a pivot and partitions the data around it. It is usually very fast, with an average complexity of O(n log n).
Heap Sort: Uses a heap data structure to repeatedly select elements. Its time complexity is O(n log n).

### Conclusion

Sorting algorithms are essential techniques in computer science used to arrange data in a specific order. Different algorithms such as **Bubble Sort, Selection Sort, Insertion Sort, Merge Sort, and Quick Sort** have different approaches and performance levels. Simple algorithms are easy to understand and implement, while advanced algorithms like Merge Sort and Quick Sort are more efficient for handling large amounts of data. Therefore, choosing the appropriate sorting algorithm depends on the **size of the data, time complexity, memory requirements, and application**. Overall, understanding sorting algorithms helps in developing efficient and well-organized computer programs.



practical-2
summary:

**Linear Search** checks each element one by one from the beginning until the required element is found or the list ends. It is simple and works even when the data is **unsorted**, but it can be slow for large datasets. Its time complexity is **O(n)**.

**Binary Search** is a faster searching technique that works only on **sorted data**. It repeatedly divides the search range into two halves and compares the middle element with the target. Its time complexity is **O(log n)**, making it much more efficient for large datasets.

Conclusion

In conclusion, both Linear Search and Binary Search are important searching algorithms. **Linear Search** is easier to implement and is useful for small or unsorted data, while **Binary Search** is more efficient for large, sorted datasets. Choosing the appropriate algorithm depends on the size and organization of the data and the required performance.


practical-3
Summary

**Max Heap, Min Heap, and Heap Sort** are important concepts in data structures and algorithms. A **Max Heap** is a complete binary tree in which the parent node is greater than or equal to its children, so the largest element is always at the root. A **Min Heap** is a complete binary tree in which the parent node is smaller than or equal to its children, making the smallest element the root.

**Heap Sort** uses a heap structure to arrange elements in sorted order. It can be performed using a Max Heap for ascending order or a Min Heap for descending order. Heap Sort has a time complexity of **O(n log n)** and does not require extra memory proportional to the input size.

 Conclusion

In conclusion, **Max Heap and Min Heap** provide efficient ways to organize and access the largest or smallest elements. **Heap Sort** uses these properties to sort data efficiently with **O(n log n)** time complexity. Therefore, heaps are useful in sorting, priority queues, scheduling, and other applications where efficient access to maximum or minimum values is required.

practical-4
Summary = This C++ program calculates the factorial of a non-negative integer using two different approaches: iterative and recursive. It accepts user input, validates that the number is non-negative, and computes the factorial using both methods. The program also measures and compares the execution time of each approach using the chrono library with nanosecond precision. The iterative method uses a loop and requires constant extra memory, while the recursive method repeatedly calls itself until the base case is reached,consuming additional memory due to the function call stack.

Conclusion = The program demonstrates that both iterative and recursive methods produce the same factorial result for a valid input. However, the iterative approach is generally more efficient because it uses O(1) space and avoids the overhead of recursive function calls. The recursive approach is simpler and easier to understand conceptually but requires O(n) space due to recursion. Overall, this program effectively compares the performance and memory usage of both techniques while illustrating the concepts of algorithm complexity and execution time measurement.

practical-7
Summary

The given Python program solves the Making Change Problem using Dynamic Programming. It takes the number of coin denominations, the coin values, and the target amount as input. It creates a DP array where dp[i] represents the minimum number of coins needed to make the amount i. The base case is dp[0] = 0, since zero coins are needed to make amount 0. The program then checks each coin for every amount and stores the minimum number of coins required. Finally, it displays the minimum number of coins, the complete DP table, and the time and space complexities.

Conclusion

The Dynamic Programming approach provides an efficient solution to the Making Change Problem by avoiding repeated calculations and storing previously computed results. If the target amount can be formed using the given denominations, the program returns the minimum number of coins required; otherwise, it reports that change cannot be made. The algorithm has a time complexity of O(amount × number of coins) and a space complexity of O(amount), making it suitable for solving the problem efficiently for moderate-sized amounts.
# Practical 5

## Aim

# To implement the **0/1 Knapsack Problem** using the **Dynamic Programming** technique and find the maximum value that can be obtained without exceeding the given knapsack capacity.

---

## Problem Statement

The **0/1 Knapsack Problem** is an optimization problem where a set of items is given, and each item has:

- A weight
- A value

The objective is to select items such that the **total value is maximum**, while the **total weight does not exceed the capacity of the knapsack**.

Each item can be selected **only once**.

---

## Algorithm Used

### Dynamic Programming

A 2D DP table is used to solve the problem.

`dp[i][w]` represents the maximum value that can be obtained using the first `i` items with a knapsack capacity of `w`.

For every item, two choices are considered:

1. **Include the item**
2. **Exclude the item**

The maximum value from these two choices is stored in the DP table.

---

## Input

The program takes the following inputs from the user:

- Number of items
- Weight of each item
- Value of each item
- Maximum capacity of the knapsack

---

## Output

The program displays:

- Maximum value
- Selected items
- Execution time
- Time complexity
- Space complexity

practical-6

Summary
Matrix Chain Multiplication (MCM) is a Dynamic Programming problem used to find the minimum number of scalar multiplications needed to multiply a sequence of matrices.
The goal is not to multiply the matrices, but to find the best order (parenthesization) for multiplication.


Conclusion:
Matrix Chain Multiplication is an efficient Dynamic Programming technique used to determine the best order for multiplying a sequence of matrices. It reduces the total number of scalar multiplications by dividing the problem into smaller subproblems and storing their results.

 Practical-8

This directory contains the Python implementation of core graph traversal algorithms: **Depth-First Search (DFS)** and **Breadth-First Search (BFS)** on undirected graphs represented via an **Adjacency List**. The program measures and compares execution runtimes using `time.perf_counter()`.

---

## 📌 Problem Overview & Concepts

Graph traversal refers to the process of visiting all the vertices (nodes) in a graph systematic search pattern.

### Graph Representation
The graph is represented using an **Adjacency List** using Python's `collections.defaultdict(list)` for efficient $\mathcal{O}(1)$ neighbor lookup and $\mathcal{O}(V + E)$ space complexity.

### Algorithms Implemented

1. **Depth-First Search (DFS) (`dfs(start)`)**
   - Traverses deeply along each branch of the graph before backtracking.
   - Uses recursion (implicit call stack) to keep track of visited nodes.
   - **Time Complexity:** $\mathcal{O}(V + E)$ where $V$ is the number of vertices and $E$ is the number of edges.
   - **Space Complexity:** $\mathcal{O}(V)$ due to the boolean `visited` array and recursion call stack frame.
   - **Applications:** Topological sorting, detecting cycles, connected components, solving mazes/puzzles.

2. **Breadth-First Search (BFS) (`bfs(start)`)**
   - Explores nodes level-by-level, visiting all immediate neighbors of a vertex before proceeding to the next level.
   - Uses an explicit First-In-First-Out (FIFO) queue (`collections.deque`) to manage node exploration.
   - **Time Complexity:** $\mathcal{O}(V + E)$
   - **Space Complexity:** $\mathcal{O}(V)$ for storing nodes in the queue and visited array.
   - **Applications:** Shortest path in unweighted graphs, web crawlers, social network connection levels (degrees of separation), minimum spanning tree (Bipartite testing).

---

## ⚡ Complexity Summary

| Algorithm | Time Complexity | Auxiliary Space | Underlying Data Structure | Exploration Strategy |
| :--- | :---: | :---: | :---: | :--- |
| **Depth-First Search (DFS)** | $\mathcal{O}(V + E)$ | $\mathcal{O}(V)$ | Recursion Stack | Deep-first / Branch-by-branch |
| **Breadth-First Search (BFS)** | $\mathcal{O}(V + E)$ | $\mathcal{O}(V)$ | FIFO Queue (`deque`) | Level-by-level / Radial |

---

## 💻 How to Run

1. Open your terminal or command prompt.
2. Navigate to the `practical_8` directory:
   ```bash
   cd practical_8
   ```
3. Execute the Python script:
   ```bash
   python graph_traversal.py
   ```

---

## 📋 Sample Input & Output

### Input Example (Graph with 5 Vertices and 6 Edges):
```text
Enter number of vertices: 5
Enter number of edges: 6
Enter edges (u v):
0 1
0 2
1 3
1 4
2 4
3 4
Enter starting vertex: 0
```

### Execution Output:
```text
DFS Traversal: 0 1 3 4 2
BFS Traversal: 0 1 2 3 4

Execution Time:
DFS: 5399.98 ns
BFS: 7900.00 ns

=======================================================
         GRAPH TRAVERSAL COMPLEXITY SUMMARY
=======================================================
Method     | Time Complexity    | Space Complexity  
-------------------------------------------------------
DFS        | O(V + E)           | O(V)              
BFS        | O(V + E)           | O(V)              
=======================================================
```

---

## 📖 Key Takeaways & Conclusion

1. **Traversal Paradigms**:
   - **DFS** dives deep into a single branch until dead-end before backtracking, making it ideal for path-finding, topological ordering, and constraint satisfaction.
   - **BFS** expands uniformly outwards level-by-level, guaranteeing the shortest path in unweighted graphs.
2. **Efficiency**:
   - Both DFS and BFS achieve linear time complexity $\mathcal{O}(V + E)$ relative to graph size, making them optimal search methods for arbitrary graph topologies.
