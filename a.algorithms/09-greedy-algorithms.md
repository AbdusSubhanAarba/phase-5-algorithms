# Greedy Algorithms

## Overview

A Greedy Algorithm is a problem-solving approach that makes the **best possible choice at each step**, hoping that these local optimal choices will lead to the overall best solution.

Instead of considering every possible solution, a greedy algorithm always chooses what seems to be the best option **right now** without changing previous decisions.

Greedy algorithms are fast and efficient, but they do not always produce the optimal solution for every problem.

---

## Why It Matters

Greedy algorithms are important because they:

- Solve many optimization problems efficiently
- Are simple to understand and implement
- Often produce fast solutions
- Reduce computation time
- Are widely used in networking, scheduling, and graph algorithms

Many real-world systems rely on greedy strategies because of their speed.

---

## How Greedy Algorithms Work

A greedy algorithm follows one simple rule:

**At every step, choose the option that looks best at that moment.**

Once a decision is made, it is never changed.

Unlike some other algorithms, greedy algorithms do not look ahead or reconsider previous choices.

---

## Example: Coin Change

Imagine you need to make:

```text
87 cents
```

Available coins:

```text
50¢

25¢

10¢

1¢
```

A greedy algorithm chooses:

```text
50¢

↓

25¢

↓

10¢

↓

1¢

↓

1¢
```

Total:

```text
87¢
```

At every step, it chooses the largest possible coin.

---

## Example: Choosing Activities

Suppose you want to attend as many meetings as possible.

Meetings:

```text
9:00–10:00

10:00–11:00

10:30–12:00

12:00–1:00
```

A greedy algorithm chooses the meeting that finishes earliest.

This leaves the most time available for the remaining meetings.

---

## Greedy Choice Property

Greedy algorithms work well only when a problem has the **Greedy Choice Property**.

This means:

Making the best choice now will eventually lead to the best overall solution.

Not every problem has this property.

---

## Greedy vs Dynamic Programming

Both solve optimization problems, but they work differently.

### Greedy Algorithm

- Makes the best immediate choice.
- Never changes previous decisions.
- Usually faster.
- Simpler to implement.

---

### Dynamic Programming

- Examines multiple possibilities.
- Stores previous results.
- Guarantees the optimal solution for many problems.
- Usually requires more memory and computation.

Dynamic Programming is more powerful, while Greedy Algorithms are often faster.

---

## Advantages of Greedy Algorithms

Greedy algorithms provide several benefits:

- Fast execution
- Simple implementation
- Low memory usage
- Efficient for many optimization problems
- Easy to understand

---

## Disadvantages of Greedy Algorithms

Greedy algorithms also have limitations:

- Do not always produce the optimal solution.
- Cannot solve every optimization problem.
- Never reconsider previous decisions.
- Choosing the locally best option may lead to a poor overall result.

Because of this, greedy algorithms must only be used when the problem satisfies the Greedy Choice Property.

---

## Real-World Examples

Greedy algorithms are used in many applications.

### GPS Navigation

Choosing the next road that appears to move closer to the destination.

---

### CPU Scheduling

Selecting the shortest available job first.

---

### Network Routing

Finding efficient paths through computer networks.

---

### Data Compression

Huffman Coding uses a greedy algorithm to compress files efficiently.

---

### Minimum Spanning Tree

Algorithms such as:

- Kruskal's Algorithm
- Prim's Algorithm

use greedy strategies to build efficient network connections.

---

## Time Complexity

The time complexity depends on the specific greedy algorithm.

Examples include:

| Algorithm | Time Complexity |
|-----------|----------------:|
| Activity Selection | O(n log n) |
| Kruskal's Algorithm | O(E log E) |
| Prim's Algorithm | O(E log V) |
| Huffman Coding | O(n log n) |

There is no single time complexity for all greedy algorithms.

---

## Greedy Algorithms vs Brute Force

| Greedy Algorithm | Brute Force |
|------------------|-------------|
| Chooses the best option immediately | Tries every possible solution |
| Fast | Usually slow |
| May not find the optimal solution | Always finds the optimal solution (if enough time) |
| Efficient | Computationally expensive |

Greedy algorithms sacrifice completeness for speed.

---

## Common Mistakes Beginners Make

Beginners often:

- Assume greedy algorithms always find the best solution.
- Confuse greedy algorithms with dynamic programming.
- Ignore whether the problem satisfies the Greedy Choice Property.
- Think the locally best choice is always the globally best choice.

Understanding the problem is more important than simply applying a greedy strategy.

---

## Key Takeaways

- Greedy algorithms choose the best immediate option at every step.
- Previous decisions are never changed.
- They are fast and memory-efficient.
- They work well only for certain types of problems.
- Many optimization problems use greedy algorithms successfully.
- They do not always produce the optimal solution.

---

## Summary

Greedy algorithms solve problems by making the best possible decision at each step without reconsidering previous choices. This approach makes them fast, simple, and efficient for many optimization problems, including scheduling, networking, and data compression. However, because greedy algorithms focus only on the current best choice, they do not always guarantee the optimal overall solution. Understanding when a greedy approach is appropriate is an essential skill in algorithm design.
