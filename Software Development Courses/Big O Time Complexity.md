### What is Big O and what does it help explain about algorithms?

Big O is a method to categorize algorithms based on their time complexity or memory performance as input grows

### What are the three key concepts for understanding time complexity in Big O notation?

- Growth with respect to input, 
- Constants are always dropped
- Consider worst-case scenario when analyzing algorithm performance

### How can you quickly determine the Big O complexity of an algorithm
Looks for loops that iterate over the input. The number and nature of loops indicate the algorithm's time complexity, suck as counting nested loops or iterations through input elements.

### What are some common time complexity classifications in Big O notation?

Common time complexities include: 
- O(1) - constant time
- O(log n)- logarithmic time
- O(n) - Linear time
- O($n^2$) - quadratic time
- O($n^3$) - cubic time
- Exponential time complexities

### Why do we drop constants in Big O notation?
 Constants are dropped because Big O focuses on the algorithm's growth trend as input size increases. The relative growth of different complexity classes (like N vs N$^2$) becomes more significant than small constant multipliers.