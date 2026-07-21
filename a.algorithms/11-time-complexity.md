# Time Complexity

## Overview

Time Complexity is a way of measuring how the running time of an algorithm changes as the size of the input grows. Instead of measuring time in seconds, time complexity describes **how efficiently an algorithm performs** as more data is processed.

It allows software engineers to compare algorithms and choose the most efficient solution for a given problem.

---

## Why It Matters

Time complexity is important because it:

- Measures algorithm efficiency
- Helps compare different algorithms
- Predicts performance on large datasets
- Helps optimize software
- Reduces execution time
- Is essential in technical interviews and software engineering

An algorithm that works well for 10 items may perform very poorly with 10 million items.

---

## Input Size (n)

Time complexity is usually written using **n**, where:

```text
n = Number of input elements
```

Example:

```text
10 numbers

↓

n = 10
```

```text
1,000 numbers

↓

n = 1,000
```

As **n** increases, the algorithm performs more work.

---

## Why We Don't Measure Seconds

Instead of saying:

```text
"This algorithm takes 2 seconds."
```

We focus on how performance changes as the input grows.

Different computers have different speeds.

Time complexity measures **growth**, making it independent of hardware.

---

## Common Time Complexities

### O(1) — Constant Time

The running time never changes, regardless of the input size.

Example:

Accessing an array element by index.

```text
Array

[10, 20, 30]

Access index 1

↓

20
```

Only one operation is required.

---

### O(log n) — Logarithmic Time

The algorithm repeatedly cuts the problem in half.

Example:

Binary Search.

```text
1000 items

↓

500

↓

250

↓

125

↓

...
```

The search space becomes smaller very quickly.

---

### O(n) — Linear Time

The algorithm examines each element once.

Example:

Linear Search.

```text
1

↓

2

↓

3

↓

4

↓

...
```

If the input doubles, the work roughly doubles.

---

### O(n log n) — Linearithmic Time

The algorithm processes every element while repeatedly dividing the problem.

Examples:

- Merge Sort
- Quick Sort (Average Case)

This is considered very efficient for sorting large datasets.

---

### O(n²) — Quadratic Time

Every element is compared with many other elements.

Example:

Bubble Sort.

```text
1 ↔ 2

1 ↔ 3

1 ↔ 4

2 ↔ 3

2 ↔ 4

3 ↔ 4
```

As the input grows, the number of comparisons increases rapidly.

---

### O(2ⁿ) — Exponential Time

The amount of work doubles with every additional input.

Example:

Naive recursive Fibonacci.

Algorithms with exponential complexity become extremely slow even for moderate input sizes.

---

## Visual Comparison

```text
Fastest

O(1)

↓

O(log n)

↓

O(n)

↓

O(n log n)

↓

O(n²)

↓

O(2ⁿ)

Slowest
```

Smaller growth rates generally lead to better performance.

---

## Real-World Examples

### O(1)

Opening a contact using its exact index.

---

### O(log n)

Searching for a word in a dictionary.

---

### O(n)

Reading every email in your inbox.

---

### O(n log n)

Sorting thousands of products by price.

---

### O(n²)

Comparing every student with every other student.

---

## Why Efficient Algorithms Matter

Imagine searching through:

```text
10 items
```

Almost any algorithm performs well.

Now imagine:

```text
10,000,000 items
```

An inefficient algorithm may take minutes or even hours, while an efficient one finishes in seconds.

This is why time complexity is so important in software engineering.

---

## Time Complexity of Common Algorithms

| Algorithm | Time Complexity |
|-----------|----------------:|
| Array Access | O(1) |
| Linear Search | O(n) |
| Binary Search | O(log n) |
| Bubble Sort | O(n²) |
| Selection Sort | O(n²) |
| Merge Sort | O(n log n) |
| Quick Sort (Average) | O(n log n) |

---

## Common Mistakes Beginners Make

Beginners often:

- Think time complexity measures actual seconds.
- Focus only on small datasets.
- Assume every fast algorithm has O(1) complexity.
- Ignore how quickly algorithms scale as input grows.
- Memorize complexities without understanding why they occur.

Understanding the growth pattern is more important than memorizing values.

---

## Key Takeaways

- Time complexity measures how an algorithm's running time grows.
- It depends on the size of the input (**n**).
- It is independent of computer speed.
- Lower time complexity generally means better performance.
- Efficient algorithms become increasingly important as datasets grow.
- Big-O notation is commonly used to express time complexity.

---

## Summary

Time complexity is one of the most important concepts in computer science because it measures how efficiently an algorithm performs as the input size increases. Rather than measuring time in seconds, it focuses on the growth of the algorithm's workload. Understanding time complexity allows software engineers to compare algorithms, optimize performance, and build applications that remain fast and scalable even when processing large amounts of data.
