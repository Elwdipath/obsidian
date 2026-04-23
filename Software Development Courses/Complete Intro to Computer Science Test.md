# Complete Intro to Computer Science  
## 50-Question Intermediate Multiple-Choice Test

**Instructions:**  
Select the best answer for each question.

---

## Section 2: Algorithm Analysis

1. What does Big O notation describe?
   - [ ] A. Exact execution time
   - [ ] B. Memory usage only
   - [ ] C. Algorithm growth rate as input increases
   - [ ] D. Compiler optimization level

2. Why are constant factors ignored in Big O?
   - [ ] A. They are unpredictable
   - [ ] B. They dominate performance
   - [ ] C. They don’t affect growth rate
   - [ ] D. They depend on hardware

3. Which grows fastest as input size increases?
   - [ ] A. O(log n)
   - [ ] B. O(n)
   - [ ] C. O(1)
   - [ ] D. O(n²)

4. What is the time complexity of looping once through an array?
   - [ ] A. O(1)
   - [ ] B. O(log n)
   - [ ] C. O(n)
   - [ ] D. O(n²)

5. What is the space complexity of creating a new array of size `n`?
   - [ ] A. O(1)
   - [ ] B. O(log n)
   - [ ] C. O(n)
   - [ ] D. O(n²)

6. Why is worst-case complexity preferred?
   - [ ] A. It happens most often
   - [ ] B. It gives a guaranteed upper bound
   - [ ] C. Average case is always slower
   - [ ] D. Hardware varies too much

7. `O(n + n²)` simplifies to:
   - [ ] A. O(n)
   - [ ] B. O(n log n)
   - [ ] C. O(n²)
   - [ ] D. O(2n)

8. Which is an example of a time/space tradeoff?
   - [ ] A. Sorting faster using less memory
   - [ ] B. Using caching to speed lookups
   - [ ] C. Writing fewer lines of code
   - [ ] D. Using recursion instead of loops

---

## Section 3: Iterative Sorts

9. Bubble Sort works by:
   - [ ] A. Dividing the array recursively
   - [ ] B. Selecting a pivot
   - [ ] C. Repeatedly swapping adjacent elements
   - [ ] D. Using buckets

10. Worst-case time complexity of Bubble Sort:
    - [ ] A. O(n)
    - [ ] B. O(n log n)
    - [ ] C. O(n²)
    - [ ] D. O(log n)

11. Why is Bubble Sort rarely used?
    - [ ] A. Hard to implement
    - [ ] B. Requires recursion
    - [ ] C. Inefficient on large datasets
    - [ ] D. Uses too much memory

12. Bubble Sort performs best when:
    - [ ] A. Data is reverse-sorted
    - [ ] B. Data is random
    - [ ] C. Data is nearly sorted
    - [ ] D. Data contains duplicates

13. Insertion Sort works by:
    - [ ] A. Swapping random elements
    - [ ] B. Inserting elements into a growing sorted portion
    - [ ] C. Splitting arrays recursively
    - [ ] D. Counting values

14. Best-case time complexity of Insertion Sort:
    - [ ] A. O(n²)
    - [ ] B. O(n log n)
    - [ ] C. O(n)
    - [ ] D. O(log n)

15. Why is Insertion Sort good for small datasets?
    - [ ] A. No comparisons
    - [ ] B. Low overhead
    - [ ] C. Uses hashing
    - [ ] D. Parallel execution

16. Which is generally faster?
    - [ ] A. Bubble Sort
    - [ ] B. Insertion Sort
    - [ ] C. They are equal
    - [ ] D. Depends on hardware only

---

## Section 4: Recursive Sorts

17. Recursion requires:
    - [ ] A. A loop and condition
    - [ ] B. A stack and heap
    - [ ] C. A base case and recursive case
    - [ ] D. Sorting first

18. Missing a base case causes:
    - [ ] A. Slow performance
    - [ ] B. Stack overflow
    - [ ] C. Incorrect sorting
    - [ ] D. Memory leaks only

19. Merge Sort works by:
    - [ ] A. Swapping adjacent values
    - [ ] B. Partitioning around a pivot
    - [ ] C. Dividing and merging sorted halves
    - [ ] D. Counting digits

20. Time complexity of Merge Sort:
    - [ ] A. O(n)
    - [ ] B. O(n²)
    - [ ] C. O(n log n)
    - [ ] D. O(log n)

21. Merge Sort space complexity is:
    - [ ] A. O(1)
    - [ ] B. O(log n)
    - [ ] C. O(n)
    - [ ] D. O(n²)

22. Quick Sort pivot selection:
    - [ ] A. Always first element
    - [ ] B. Always last element
    - [ ] C. Arbitrary element
    - [ ] D. Random or chosen strategy

23. Average-case time complexity of Quick Sort:
    - [ ] A. O(n)
    - [ ] B. O(n log n)
    - [ ] C. O(n²)
    - [ ] D. O(log n)

24. Worst-case Quick Sort occurs when:
    - [ ] A. Data is random
    - [ ] B. Pivot is poorly chosen
    - [ ] C. Data is small
    - [ ] D. Using recursion

25. Why is Quick Sort often fast in practice?
    - [ ] A. No recursion
    - [ ] B. Better cache locality
    - [ ] C. Guaranteed balance
    - [ ] D. Uses less comparisons always

---

## Section 5: Non-Comparison Sorts

26. Radix Sort differs because it:
    - [ ] A. Uses recursion
    - [ ] B. Compares values directly
    - [ ] C. Sorts by digit position
    - [ ] D. Uses trees

27. Radix Sort works best on:
    - [ ] A. Floating-point numbers
    - [ ] B. Arbitrary objects
    - [ ] C. Integers or fixed-length strings
    - [ ] D. Graphs

28. Radix Sort time complexity depends on:
    - [ ] A. Input randomness
    - [ ] B. Number of digits and items
    - [ ] C. Pivot choice
    - [ ] D. Tree depth

29. Why isn’t Radix Sort universal?
    - [ ] A. Uses too much memory
    - [ ] B. Only works on specific data types
    - [ ] C. Too slow
    - [ ] D. Requires recursion

---

## Section 6: Binary Search

30. Binary Search requires:
    - [ ] A. Linked list
    - [ ] B. Sorted data
    - [ ] C. Hashing
    - [ ] D. Recursion only

31. Binary Search reduces search space by:
    - [ ] A. One element
    - [ ] B. One third
    - [ ] C. Half
    - [ ] D. Random amount

32. Binary Search time complexity:
    - [ ] A. O(1)
    - [ ] B. O(n)
    - [ ] C. O(log n)
    - [ ] D. O(n log n)

33. Binary Search is faster than linear search because it:
    - [ ] A. Uses recursion
    - [ ] B. Eliminates half the data each step
    - [ ] C. Uses pointers
    - [ ] D. Avoids comparisons

---

## Section 7: Lists

34. ArrayList stores data:
    - [ ] A. Non-contiguously
    - [ ] B. In nodes
    - [ ] C. Contiguously
    - [ ] D. In trees

35. ArrayList index access:
    - [ ] A. O(n)
    - [ ] B. O(log n)
    - [ ] C. O(1)
    - [ ] D. O(n log n)

36. LinkedList insertion at head:
    - [ ] A. O(n)
    - [ ] B. O(log n)
    - [ ] C. O(1)
    - [ ] D. O(n²)

37. Random access in LinkedList is slow because:
    - [ ] A. Uses recursion
    - [ ] B. Nodes are scattered
    - [ ] C. Needs traversal
    - [ ] D. Uses hashing

38. LinkedList is preferred when:
    - [ ] A. Frequent random access
    - [ ] B. Frequent inserts/deletes
    - [ ] C. Data is sorted
    - [ ] D. Memory is limited

---

## Section 8: Trees

39. A Binary Search Tree property:
    - [ ] A. Balanced always
    - [ ] B. Left < node < right
    - [ ] C. Heap ordered
    - [ ] D. Sorted array

40. Unbalanced BST performance becomes:
    - [ ] A. O(1)
    - [ ] B. O(log n)
    - [ ] C. O(n)
    - [ ] D. O(n log n)

41. AVL Trees solve:
    - [ ] A. Sorting
    - [ ] B. Balancing
    - [ ] C. Searching arrays
    - [ ] D. Hashing

42. AVL Trees rebalance using:
    - [ ] A. Swaps
    - [ ] B. Merges
    - [ ] C. Rotations
    - [ ] D. Buckets

43. DFS differs from BFS because DFS:
    - [ ] A. Uses a queue
    - [ ] B. Uses recursion or stack
    - [ ] C. Is always faster
    - [ ] D. Sorts nodes

44. DFS traversal types:
    - [ ] A. Left, Right
    - [ ] B. In, Pre, Post order
    - [ ] C. Level order only
    - [ ] D. Random order

45. A binary heap property:
    - [ ] A. Sorted structure
    - [ ] B. Parent ordered relative to children
    - [ ] C. Balanced search tree
    - [ ] D. Linked list

46. Heap Sort time complexity:
    - [ ] A. O(n)
    - [ ] B. O(log n)
    - [ ] C. O(n log n)
    - [ ] D. O(n²)

---

## Section 9: Trees Applied

47. Graphs differ from trees because graphs:
    - [ ] A. Have roots
    - [ ] B. Can contain cycles
    - [ ] C. Are always directed
    - [ ] D. Cannot branch

48. Dijkstra’s algorithm finds:
    - [ ] A. Minimum spanning tree
    - [ ] B. All cycles
    - [ ] C. Shortest path
    - [ ] D. Maximum flow

49. Tries optimize:
    - [ ] A. Numeric sorting
    - [ ] B. Graph traversal
    - [ ] C. Prefix searching
    - [ ] D. Hash collisions

---

## Section 10: Bloom Filters

50. Bloom Filters trade:
    - [ ] A. Speed for accuracy
    - [ ] B. Accuracy for memory efficiency
    - [ ] C. Space for time
    - [ ] D. Sorting for hashing
