### What is the fundamental definition of an array in terms of computer memory?
A contiguous memory space containing zero or more pieces of memory understood as a single type in a row, where elements can be accessed by calculating memory offset based on type size and index

### What is the time complexity for accessing an element in an array by its index?
O(1) or constant time, because the memory location can be directly calculated without iterating through the entire array

### What limitation exists when inserting elements into a traditional array?
Arrays cannot dynamically grow in memory. Insertion typically overwrites existing elements, and attempting to expand beyond the original memory allocation could overwrite adjacent memory locations

### How does an array handle deletion of an element?
Deletion typically involves setting the element to a sentinel value like zero, but does not actually remove the memory space, The programmer must manage how deleted elements are interpreted.

### What determines how memory is interpreted in an array?
The type of view or interpretation applied to the memory, such as an 8-bit unsigned integer view versus a 16-bit unsigned integer view, which can change how the same memory bytes are understood

### What characteristic defines a traditional array's size?
A traditional array must have its size specified at initialization and cannot dynamically grow; the size is fixed and must be determined when the array is created

### What happens when you want to increase the size of a traditional array?
You must reallocate a new array, create a new larger array, and coppy the contents of the old array into the new one

### What are the key components needed when defining and array in older languages?
In older languages, you need to pass three key pieces: 
- The type of data
- A pointer to the beginning of the array 
- The length of the array

### What considerations are important when determining the initial size of an array's memory buffer?
The initial buffer size must balance between having enough space to avoid frequent reallocation and not wasting excessive memory by creating an overly large buffer

### What are the different types of array size specification in programming languages?
Arrays can have variable sizes (determined at runtime) or compile-time fixes sizes (where the size is a constant known before program execution)
