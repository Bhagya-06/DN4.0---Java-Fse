# 📈 Financial Forecasting Tool

In this exercise, we implement a **recursive algorithm** to forecast future financial values based on past data.



## 🎯 Objective

To build a simple forecasting model that:
- Uses **recursion** to simulate compound growth
- Predicts the future value of an amount over time
- Analyzes time complexity and potential optimizations


## 📘 1. Understanding Recursive Algorithms

### ➤ What is Recursion?

Recursion is a programming technique where a method **calls itself** to solve smaller instances of the same problem. It is particularly useful for problems that are **defined in terms of their smaller subproblems**, such as:

- Factorials
- Fibonacci numbers
- Compound growth (as in financial forecasting)



## 🏗️ 2. Setup

A recursive method is created to calculate the **future value** of a financial amount based on:

- `initialAmount` — the starting value
- `growthRate` — annual growth rate (as a decimal)
- `years` — number of years into the future



## 🔁 3. Implementation Logic

The future value is calculated recursively using the following formula:
- FutureValue(n) = FutureValue(n - 1) * (1 + growthRate)
- Base Case: FutureValue(0) = initialAmount

Each year builds upon the value of the **previous year**, representing **compound growth**.



## 📊 4. Algorithm Analysis

### ➤ Time Complexity:

- **Recursive approach** has a time complexity of **O(n)**, where `n` is the number of years.
- Each recursive call reduces the problem by 1 year, so the number of calls grows linearly.

### ➤ Optimization Suggestions:

- For small `n`, recursion is sufficient.
- For large `n`, we may consider:
  - **Memoization** to store previously computed values.
  - **Iterative approach** (using a loop) to reduce function call overhead.

