# Data Structure

Data structures refer to how data is **organized**.

### Data structure operations
* Read
* Search
* Insert
* Delete

> Read and Search difference:
> Reading refers to looking something up at  **particular spot** within the data structure.
> Search refers to looking for a **particular value** within a data structure.

### Measuring Speed
If you take away just one thing from this book, let it be this: when we measure how “fast” an operation takes, we do not refer to how fast the operation takes in terms of pure time, but instead in **how many steps it takes.**

--- 
### Array
* When a program declares an array, it allocates a **contiguous** set of empty cells for use in the program.
* **Reading** an array is fast and it only take one step.
* **Searching** is less efficent than reading, since the computer have to check all cells until it find the value.
* **Insertion**: It depends on **where** within the array you're inserting it. The worse-case is when we insert data at the **beginning** of the array. (N+1 steps)
* **Deletion**: It take two steps: (1) Delete the target one. (2) Shift remaining elements to close the gap. The worse-case is deleting the first element of the array.

---
### Sets
A set never allows duplicate values to be contained within it.

* **Reading**: The Time Complexity is exactly the same as an classic array.
* **Searching**: Same as an array too, it takes up to N steps to search for a value. So is **Deletion**.
* **Insertion**: The computer needs to search N celles to ensure that the set doesn't already contain that value,  another N steps to shift all the data to the right, and another final steps to insert the new value. That's a total of **2N + 1 steps.**

