# Selection Sort

## Overview

Selection Sort is a simple sorting algorithm that repeatedly finds the **smallest element** from the unsorted portion of a collection and places it into its correct position.

Unlike Bubble Sort, which performs many swaps, Selection Sort performs **only one swap per pass**, making it more efficient in terms of the number of swaps.

Although it is easy to understand, Selection Sort is still inefficient for large datasets.

---

## Why It Matters

Selection Sort is important because it:

- Introduces another approach to sorting
- Demonstrates how selecting minimum values works
- Performs fewer swaps than Bubble Sort
- Builds a foundation for understanding more advanced sorting algorithms

It is commonly used for educational purposes.

---

## How Selection Sort Works

Selection Sort divides the collection into two parts:

- **Sorted portion**
- **Unsorted portion**

During each pass:

1. Find the smallest element in the unsorted portion.
2. Swap it with the first unsorted element.
3. Expand the sorted portion.
4. Repeat until every element is sorted.

---

## Example

Suppose we have the following array:

```text
[64, 25, 12, 22, 11]
```

### Pass 1

Find the smallest value:

```text
11
```

Swap with the first element.

```text
[11, 25, 12, 22, 64]
```

---

### Pass 2

Ignore the already sorted element.

Find the smallest remaining value:

```text
12
```

Swap.

```text
[11, 12, 25, 22, 64]
```

---

### Pass 3

Find the smallest remaining value:

```text
22
```

Swap.

```text
[11, 12, 22, 25, 64]
```

---

### Pass 4

Only one element remains.

The array is now sorted.

```text
[11, 12, 22, 25, 64]
```

---

## Visual Example

Before:

```text
64  25  12  22  11
```

↓

```text
11  25  12  22  64
```

↓

```text
11  12  25  22  64
```

↓

```text
11  12  22  25  64
```

↓

```text
11  12  22  25  64 ✅
```

Each pass places one element into its final position.

---

## Advantages of Selection Sort

Selection Sort provides several benefits:

- Easy to understand
- Simple implementation
- Performs fewer swaps than Bubble Sort
- Requires very little extra memory

---

## Disadvantages of Selection Sort

Selection Sort also has some limitations:

- Slow for large datasets
- Still performs many comparisons
- Not suitable for high-performance applications

Modern sorting algorithms are much faster for large collections.

---

## Real-World Examples

Selection Sort is useful for:

- Learning sorting algorithms
- Small datasets
- Situations where minimizing swaps is important
- Teaching algorithm design

It is rarely used in production software.

---

## Time Complexity

| Case | Time Complexity |
|------|----------------:|
| Best Case | O(n²) |
| Average Case | O(n²) |
| Worst Case | O(n²) |

Unlike Bubble Sort, Selection Sort performs the same number of comparisons regardless of how sorted the data already is.

---

## Space Complexity

| Complexity |
|-----------:|
| O(1) |

Selection Sort sorts the data **in place**, requiring only a small amount of additional memory.

---

## Selection Sort vs Bubble Sort

| Selection Sort | Bubble Sort |
|----------------|-------------|
| Finds the smallest element | Swaps adjacent elements |
| One swap per pass | Many swaps per pass |
| O(n²) average | O(n²) average |
| Fewer swaps | More swaps |
| Same number of comparisons every time | Can finish early if optimized |

Although both algorithms are simple, they use different strategies.

---

## Common Mistakes Beginners Make

Beginners often:

- Confuse Selection Sort with Bubble Sort.
- Swap every time a smaller element is found.
- Forget to search the entire unsorted portion before swapping.
- Assume fewer swaps automatically make the algorithm fast.

Remember that Selection Sort waits until the smallest element has been found before performing a single swap.

---

## Key Takeaways

- Selection Sort repeatedly finds the smallest remaining element.
- Each pass places one element into its correct position.
- It performs fewer swaps than Bubble Sort.
- Average and worst-case time complexity are **O(n²)**.
- Space complexity is **O(1)**.
- It is simple but inefficient for large datasets.

---

## Summary

Selection Sort is a comparison-based sorting algorithm that repeatedly selects the smallest element from the unsorted portion of a collection and places it into its correct position. While it performs fewer swaps than Bubble Sort and requires very little additional memory, its **O(n²)** time complexity makes it unsuitable for large datasets. Nevertheless, it remains an excellent algorithm for understanding the fundamentals of sorting and algorithm design.
