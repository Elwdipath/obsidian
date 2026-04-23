---
id: Linear Search & Kata Setup
aliases: []
tags:
  - computer science
  - algorithm
  - flash cards
---
### What is the time complexity of a linear search algorithm?
O(N), which means the time complexity grows linearly with the input size. As the array grows, the search time increases proportionally

### What are the key steps in implementing a basic linear search algorithm?
 - Iterate through the array from index ) to length-1
 - Compare each element with the target ----------
 - If the target value is found, return ----------
 - If the target value is not found after checking all the elements, return false.

### What is the basic signature for a linear search function?
The function takes two arguments:
 - An array(haystack)
 - Target (needle)

Then returns a boolean indicating whether the target was found in the array

### What is the worst case scenario for a linear search?
  When the target value is not present in the array, forcing the algorithm to search through every single element before returning false.

### How does a linear search compare an array's elements to find a specific value?
  It checks each element sequentially from the beginning of the array, comparing each element with the target value until a match is found or the end of the array is reached.
