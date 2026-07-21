# Dynamic Programming (Introduction)

## Overview

Dynamic Programming (DP) is an algorithm design technique used to solve complex problems by **breaking them into smaller overlapping subproblems**, solving each subproblem only once, and storing the results for future use.

Instead of solving the same problem repeatedly, Dynamic Programming remembers previous solutions, making algorithms much faster and more efficient.

Dynamic Programming is widely used in optimization problems where efficiency is critical.

---

## Why It Matters

Dynamic Programming is important because it:

- Solves complex problems efficiently
- Eliminates unnecessary repeated calculations
- Improves algorithm performance
- Reduces execution time
- Is widely used in software engineering and competitive programming

Many difficult problems become manageable with Dynamic Programming.

---

## How Dynamic Programming Works

Dynamic Programming follows three main steps:

1. Break the problem into smaller subproblems.
2. Solve each subproblem once.
3. Store the solution so it can be reused later.

Instead of solving the same problem repeatedly, the algorithm simply retrieves the stored answer.

---

## Overlapping Subproblems

Dynamic Programming works best when a problem contains **overlapping subproblems**.

This means the same smaller problem appears multiple times.

Example:

Instead of calculating:

```text
Fibonacci(3)
```

many times,

Dynamic Programming calculates it once and remembers the answer.

---

## Optimal Substructure

Dynamic Programming also requires **optimal substructure**.

This means:

The optimal solution to a large problem can be built from the optimal solutions of its smaller subproblems.

Many optimization problems have this property.

---

## Example: Fibonacci Numbers

The Fibonacci sequence is:

```text
0

1

1

2

3

5

8

13
```

Without Dynamic Programming:

```text
Fibonacci(5)

↓

Fibonacci(4)

↓

Fibonacci(3)

↓

Fibonacci(2)
```

Some values are calculated multiple times.

---

Using Dynamic Programming:

```text
Fibonacci(2)

↓

Store Result

↓

Reuse Later
```

Each value is calculated only once.

---

## Memoization

One way to implement Dynamic Programming is **Memoization**.

Memoization stores the results of previously solved subproblems.

Example:

```text
Solve Problem

↓

Store Answer

↓

Need It Again?

↓

Use Stored Answer
```

This avoids unnecessary calculations.

---

## Tabulation

Another approach is **Tabulation**.

Instead of starting with the large problem, Tabulation starts with the smallest problems and builds the solution step by step.

Example:

```text
Solve Small Problem

↓

Store Result

↓

Build Larger Solution

↓

Final Answer
```

Both Memoization and Tabulation solve the same problem using different approaches.

---

## Dynamic Programming vs Greedy Algorithms

Although both solve optimization problems, they work differently.

### Dynamic Programming

- Considers multiple possibilities.
- Stores previous results.
- Guarantees the optimal solution for many problems.
- Uses additional memory.

---

### Greedy Algorithm

- Chooses the best immediate option.
- Never changes previous decisions.
- Faster in many situations.
- Does not always produce the optimal solution.

Dynamic Programming focuses on finding the best overall solution.

---

## Advantages of Dynamic Programming

Dynamic Programming provides several benefits:

- Eliminates repeated calculations
- Produces optimal solutions for many problems
- Greatly improves efficiency
- Solves complex optimization problems
- Widely used in advanced algorithms

---

## Disadvantages of Dynamic Programming

Dynamic Programming also has some limitations:

- More difficult to understand
- Uses additional memory
- Can be complex to implement
- Not every problem can be solved using DP

It should only be used when a problem has overlapping subproblems and optimal substructure.

---

## Real-World Examples

Dynamic Programming is used in many applications.

### GPS Navigation

Finding the shortest or fastest route.

---

### Finance

Optimizing investments and minimizing costs.

---

### Robotics

Finding the most efficient movement path.

---

### Artificial Intelligence

Decision-making and optimization.

---

### Text Processing

Spell checking and text comparison algorithms.

---

## Time Complexity

The time complexity depends on the specific problem.

Examples include:

| Problem | Time Complexity |
|---------|----------------:|
| Fibonacci (Naive Recursion) | O(2ⁿ) |
| Fibonacci (Dynamic Programming) | O(n) |
| Longest Common Subsequence | O(n × m) |
| 0/1 Knapsack | O(n × W) |

Dynamic Programming often transforms extremely slow algorithms into efficient ones.

---

## Dynamic Programming vs Recursion

| Dynamic Programming | Recursion |
|---------------------|-----------|
| Stores previous results | Recalculates subproblems |
| Faster for overlapping problems | May repeat the same work |
| Uses additional memory | Uses the call stack |
| Often more efficient | Simpler for some problems |

Dynamic Programming is often built on top of recursion by adding memory.

---

## Common Mistakes Beginners Make

Beginners often:

- Confuse Dynamic Programming with recursion.
- Use DP for problems that do not require it.
- Forget to store previously computed results.
- Assume every optimization problem requires DP.
- Ignore the concepts of overlapping subproblems and optimal substructure.

Understanding *when* to use Dynamic Programming is just as important as knowing *how* it works.

---

## Key Takeaways

- Dynamic Programming solves problems by storing solutions to smaller subproblems.
- It avoids repeating the same calculations.
- Two common approaches are **Memoization** and **Tabulation**.
- It works best for problems with overlapping subproblems and optimal substructure.
- Dynamic Programming often produces optimal solutions more efficiently than naive approaches.
- It is one of the most important techniques in algorithm design.

---

## Summary

Dynamic Programming is a powerful algorithm design technique that improves efficiency by solving each subproblem only once and reusing previously computed results. By combining overlapping subproblems with optimal substructure, it transforms many complex optimization problems into manageable ones. Although it can be more difficult to learn than simpler techniques, Dynamic Programming is an essential skill for software engineers and is widely used in fields such as artificial intelligence, robotics, finance, and competitive programming.
