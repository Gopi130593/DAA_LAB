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

Summary = This C++ program calculates the factorial of a non-negative integer using two different approaches: iterative and recursive. It accepts user input, validates that the number is non-negative, and computes the factorial using both methods. The program also measures and compares the execution time of each approach using the chrono library with nanosecond precision. The iterative method uses a loop and requires constant extra memory, while the recursive method repeatedly calls itself until the base case is reached,consuming additional memory due to the function call stack.

Conclusion = The program demonstrates that both iterative and recursive methods produce the same factorial result for a valid input. However, the iterative approach is generally more efficient because it uses O(1) space and avoids the overhead of recursive function calls. The recursive approach is simpler and easier to understand conceptually but requires O(n) space due to recursion. Overall, this program effectively compares the performance and memory usage of both techniques while illustrating the concepts of algorithm complexity and execution time measurement.
