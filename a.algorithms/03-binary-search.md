# Binary Search

## Overview

Binary Search is a searching algorithm that finds a value by repeatedly dividing a **sorted** collection into two halves. Instead of checking every element one by one, it compares the target value with the middle element and eliminates half of the remaining data each time.

Because it cuts the search space in half with every comparison, Binary Search is much faster than Linear Search for large datasets.

---

## Why It Matters

Binary Search is important because it:

- Searches data extremely quickly
- Reduces the number of comparisons
- Is highly efficient for large datasets
- Is widely used in databases and search systems
- Introduces the concept of divide and conquer

Many real-world applications use Binary Search behind the scenes.

---

## Requirement

Binary Search **only works on sorted data**.

Example:

```text
✅ Sorted

[5, 10, 15, 20, 25]
```

```text
❌ Not Sorted

[20, 5, 25, 10, 15]
```

If the data is not sorted, Binary Search cannot guarantee the correct result.

---

## How Binary Search Works

Binary Search follows these steps:

1. Find the middle element.
2. Compare the middle element with the target.
3. If they are equal, stop.
4. If the target is smaller, search the left half.
5. If the target is larger, search the right half.
6. Repeat until the value is found or no elements remain.

Each comparison removes half of the remaining search area.

---

## Example

Suppose we have the following sorted array:

```text
[5, 10, 15, 20, 25, 30, 35]
```

We want to find:

```text
25
```

Step 1:

```text
Middle = 20
```

Since:

```text
25 > 20
```

Ignore the left half.

Remaining:

```text
[25, 30, 35]
```

Step 2:

```text
Middle = 30
```

Since:

```text
25 < 30
```

Ignore the right half.

Remaining:

```text
[25]
```

Step 3:

```text
25 ✅ Found
```

Only three comparisons were needed.

---

## Example: Value Not Found

Array:

```text
[2, 4, 6, 8, 10, 12]
```

Search for:

```text
9
```

Binary Search checks:

```text
Middle = 6

↓

Search Right Half

↓

Middle = 10

↓

Search Left Half

↓

8

↓

Not Found
```

Eventually, no elements remain to search.

---

## Visual Example

Searching for **70**:

```text
[10 20 30 40 50 60 70 80]
```

Step 1

```text
Middle = 40

↓

Search Right Half
```

Remaining:

```text
[50 60 70 80]
```

Step 2

```text
Middle = 60

↓

Search Right Half
```

Remaining:

```text
[70 80]
```

Step 3

```text
Middle = 70

↓

Found ✅
```

Notice how half of the data disappears after every comparison.

---

## Advantages of Binary Search

Binary Search provides several benefits:

- Extremely fast
- Very efficient for large datasets
- Requires very few comparisons
- Widely used in real-world software
- Much faster than Linear Search

---

## Disadvantages of Binary Search

Binary Search also has some limitations:

- Requires sorted data
- Sorting may take additional time
- More difficult to implement than Linear Search
- Not ideal for linked lists because random access is slow

---

## Real-World Examples

Binary Search is used in many applications.

### Dictionary

Finding a word by repeatedly opening the dictionary near the middle instead of reading every page.

---

### Phone Contacts

Searching an alphabetically sorted contact list.

---

### Library

Finding a book on shelves arranged alphabetically.

---

### Databases

Large databases use Binary Search and similar techniques to retrieve records efficiently.

---

## Time Complexity

| Case | Time Complexity |
|------|----------------:|
| Best Case | O(1) |
| Average Case | O(log n) |
| Worst Case | O(log n) |

### Best Case

The target is already the middle element.

Only one comparison is needed.

---

### Worst Case

The search continues until only one element remains.

Even then, Binary Search examines very few elements compared to Linear Search.

---

## Linear Search vs Binary Search

| Linear Search | Binary Search |
|--------------|---------------|
| Works on unsorted data | Requires sorted data |
| Checks one element at a time | Divides the search space in half |
| Time Complexity: O(n) | Time Complexity: O(log n) |
| Simple implementation | More efficient for large datasets |

Binary Search sacrifices flexibility for speed.

---

## Common Mistakes Beginners Make

Beginners often:

- Forget that the data must be sorted.
- Assume Binary Search works on any collection.
- Confuse the middle index with the middle value.
- Forget to eliminate half of the search space.
- Think Binary Search is always better, even for very small datasets.

Understanding the divide-and-conquer approach is the key to mastering Binary Search.

---

## Key Takeaways

- Binary Search only works on sorted data.
- It repeatedly divides the search space in half.
- Each comparison removes half of the remaining elements.
- Best-case time complexity is **O(1)**.
- Average and worst-case time complexity are **O(log n)**.
- Binary Search is one of the fastest searching algorithms for sorted data.

---

## Summary

Binary Search is a highly efficient searching algorithm that works by repeatedly dividing a sorted collection into smaller halves until the target value is found. Because it eliminates half of the remaining data with each comparison, it performs much faster than Linear Search on large datasets. Understanding Binary Search is essential because it introduces the divide-and-conquer strategy used by many advanced algorithms in computer science.
