# Space Complexity

## Overview

Space Complexity is a measure of how much memory an algorithm uses while it is running. Just as Time Complexity measures how an algorithm's running time grows, Space Complexity measures how its memory usage grows as the input size increases.

Memory is a limited resource, so software engineers must design algorithms that use it efficiently, especially when working with large datasets or devices with limited memory.

---

## Why It Matters

Space complexity is important because it:

- Measures memory efficiency
- Helps compare algorithms
- Reduces unnecessary memory usage
- Improves software performance
- Is essential for large-scale applications
- Helps optimize programs for limited-memory devices

An algorithm may be fast but still use too much memory.

---

## Input Size (n)

Like Time Complexity, Space Complexity is usually written using **n**, where:

```text
n = Number of input elements
```

As **n** increases, the amount of memory required by an algorithm may also increase.

---

## What Uses Memory?

An algorithm may use memory for:

- Variables
- Arrays
- Objects
- Function calls
- Recursion
- Temporary data structures

The total memory required determines the algorithm's space complexity.

---

## Common Space Complexities

### O(1) — Constant Space

The algorithm uses the same amount of memory regardless of the input size.

Example:

Finding the largest number in an array while storing only one variable.

```text
largest = current maximum
```

No matter how many numbers exist, only one extra variable is needed.

---

### O(n) — Linear Space

The memory usage grows directly with the input size.

Example:

Copying an array.

```text
Original

[1, 2, 3, 4]

↓

New Copy

[1, 2, 3, 4]
```

If the array doubles in size, the extra memory also doubles.

---

### O(n²) — Quadratic Space

Memory grows very quickly as the input increases.

Example:

Creating a two-dimensional matrix.

```text
1 2 3

4 5 6

7 8 9
```

As more rows and columns are added, memory usage increases rapidly.

---

## Example 1: O(1)

Suppose we want to calculate the sum of numbers.

```text
sum = 0

Read each number

Update sum
```

Only one variable is stored.

Memory remains constant.

---

## Example 2: O(n)

Suppose we copy every value into another array.

```text
Original

[5, 10, 15]

↓

Copy

[5, 10, 15]
```

The new array requires additional memory equal to the size of the input.

---

## Recursion and Memory

Recursive algorithms use additional memory because every function call is stored on the **call stack**.

Example:

```text
Function(5)

↓

Function(4)

↓

Function(3)

↓

Function(2)

↓

Function(1)
```

Each function call occupies memory until the recursion finishes.

This is why recursion often has higher space complexity than an iterative solution.

---

## Time Complexity vs Space Complexity

| Time Complexity | Space Complexity |
|-----------------|------------------|
| Measures execution time | Measures memory usage |
| Focuses on speed | Focuses on memory |
| Uses Big-O notation | Uses Big-O notation |
| Helps optimize performance | Helps optimize memory efficiency |

Both are equally important when evaluating an algorithm.

---

## Real-World Examples

### Mobile Apps

Mobile applications must use memory carefully to avoid crashes.

---

### Video Games

Games manage textures, characters, and maps efficiently to reduce memory usage.

---

### Web Browsers

Browsers manage memory when loading multiple tabs and web pages.

---

### Operating Systems

Operating systems constantly allocate and free memory for running programs.

---

## Time vs Space Trade-Off

Sometimes improving speed requires using more memory.

Example:

A **Hash Table** uses extra memory but provides much faster searching.

Conversely, using less memory may require additional computation, making the algorithm slower.

Software engineers often balance speed and memory depending on the application's requirements.

---

## Space Complexity of Common Algorithms

| Algorithm | Space Complexity |
|-----------|-----------------:|
| Linear Search | O(1) |
| Binary Search (Iterative) | O(1) |
| Bubble Sort | O(1) |
| Selection Sort | O(1) |
| Merge Sort | O(n) |
| Quick Sort (Average) | O(log n) |
| Recursive Fibonacci | O(n) |

Different algorithms require different amounts of memory.

---

## Common Mistakes Beginners Make

Beginners often:

- Focus only on execution speed.
- Forget that recursion uses additional memory.
- Assume faster algorithms always use less memory.
- Ignore temporary data structures.
- Confuse Time Complexity with Space Complexity.

Both time and memory should be considered when choosing an algorithm.

---

## Key Takeaways

- Space Complexity measures how much memory an algorithm uses.
- It depends on the size of the input (**n**).
- Common complexities include **O(1)**, **O(n)**, and **O(n²)**.
- Recursive algorithms usually require additional memory for the call stack.
- Some algorithms trade extra memory for faster execution.
- Efficient software balances both speed and memory usage.

---

## Summary

Space Complexity measures how an algorithm's memory requirements grow as the input size increases. While some algorithms use a constant amount of memory, others require additional storage for arrays, recursion, or temporary data structures. Understanding space complexity helps software engineers build applications that are both memory-efficient and scalable, making it an essential concept in algorithm design.
