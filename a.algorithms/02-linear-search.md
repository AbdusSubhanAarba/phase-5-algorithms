# Linear Search

## Overview

Linear Search is the simplest searching algorithm. It works by checking each element in a collection **one by one** until the desired value is found or until every element has been checked.

Because it examines elements sequentially, Linear Search works on both **sorted and unsorted** data.

Although it is easy to understand and implement, it becomes slower as the amount of data grows.

---

## Why It Matters

Linear Search is important because it:

- Is simple to learn and implement
- Works on both sorted and unsorted data
- Requires no special data organization
- Introduces the concept of searching algorithms
- Serves as the foundation for understanding more advanced search algorithms

It is often the first searching algorithm taught in computer science.

---

## How Linear Search Works

Linear Search starts from the first element.

It compares each element with the target value.

If the value matches, the search stops.

If not, it moves to the next element.

The process continues until the value is found or the end of the collection is reached.

---

## Example

Suppose we have the following array:

```text
[15, 8, 27, 42, 10]
```

We want to find:

```text
42
```

Linear Search checks:

```text
15 ❌

↓

8 ❌

↓

27 ❌

↓

42 ✅
```

The value is found after checking four elements.

---

## Example: Value Not Found

Array:

```text
[5, 12, 18, 25]
```

Search for:

```text
30
```

The algorithm checks:

```text
5 ❌

↓

12 ❌

↓

18 ❌

↓

25 ❌

↓

Not Found
```

Every element must be checked before the algorithm concludes that the value does not exist.

---

## Advantages of Linear Search

Linear Search offers several benefits:

- Very easy to understand
- Simple to implement
- Works on unsorted data
- No extra memory required
- Suitable for small datasets

---

## Disadvantages of Linear Search

Linear Search also has limitations:

- Slow for large datasets
- May need to examine every element
- Less efficient than Binary Search on sorted data

As the amount of data increases, Linear Search becomes less practical.

---

## Real-World Examples

Linear Search is used in many everyday situations.

### Looking for a Book

Imagine searching for a book on a shelf where the books are randomly arranged.

You start at one end and check each book until you find the one you want.

---

### Finding a Name on Paper

Suppose you have a printed attendance sheet.

You read each name one by one until you find yours.

---

### Searching a Playlist

If your music playlist is not sorted, your music player may check songs one by one until it finds the requested track.

---

## Time Complexity

| Case | Time Complexity |
|------|----------------:|
| Best Case | O(1) |
| Average Case | O(n) |
| Worst Case | O(n) |

### Best Case

The target is the very first element.

Only one comparison is needed.

---

### Worst Case

The target is the last element or does not exist.

Every element must be checked.

---

## Linear Search vs Binary Search

| Linear Search | Binary Search |
|--------------|---------------|
| Works on unsorted data | Requires sorted data |
| Checks one element at a time | Repeatedly divides the search area in half |
| Simpler to implement | Faster for large datasets |
| Time Complexity: O(n) | Time Complexity: O(log n) |

Binary Search is much faster, but it only works on sorted data.

---

## Common Mistakes Beginners Make

Beginners often:

- Assume Linear Search requires sorted data.
- Forget to check every element before declaring "Not Found."
- Think it is efficient for very large datasets.
- Confuse it with Binary Search.

Understanding when to use Linear Search is just as important as knowing how it works.

---

## Key Takeaways

- Linear Search checks elements one by one.
- It works on both sorted and unsorted data.
- It is simple but becomes slower as data grows.
- Best-case time complexity is **O(1)**.
- Average and worst-case time complexity are **O(n)**.
- It is best suited for small datasets or unsorted collections.

---

## Summary

Linear Search is the simplest searching algorithm and works by examining each element sequentially until the target value is found or all elements have been checked. While it is easy to understand and works with any collection of data, its performance decreases as the dataset grows. Understanding Linear Search provides the foundation for learning faster searching algorithms such as Binary Search.
