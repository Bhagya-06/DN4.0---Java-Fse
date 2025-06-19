# 🛒 E-commerce Platform Search Function

In this exercise, we have to implement and analyze **search functionality** for an e-commerce platform. The focus is on comparing two search techniques **Linear Search** and **Binary Search** based on performance and applicability.



## 📌 Objective

To build a search functionality for an e-commerce platform which needs to be optimized for fast performance as well as understand how different search algorithms work.



## 📘 1. Asymptotic Notation

### ➤ What is Big O Notation?

Big O notation is used to describe the **time complexity** of algorithms, especially how the runtime grows with the size of input `n`.

It helps us evaluate:
- Efficiency
- Scalability
- Worst-case performance

### ➤ Case Scenarios for Search:

| Case Type    | Linear Search         | Binary Search         |
|--------------|------------------------|------------------------|
| Best Case    | O(1) — found at start  | O(1) — found at middle |
| Average Case | O(n/2) ≈ O(n)          | O(log n)               |
| Worst Case   | O(n)                   | O(log n)               |

❗Binary Search is generally faster but requires sorted data.



## 🏗️ 2. Setup

### Product Class Attributes:
- `productId` (int)
- `productName` (String)
- `category` (String)

These attributes are used to search and filter products.



## 🔁 3. Implementation Overview

- **Linear Search**:
  - Works on an unsorted array
  - Iterates through each element until a match is found
- **Binary Search**:
  - Requires a sorted array (sorted by productId)
  - Uses a divide-and-conquer approach for faster lookup



## 📊 4. Algorithm Analysis

| Algorithm     | Time Complexity | When to Use                            |
|---------------|-----------------|----------------------------------------|
| Linear Search | O(n)            | Small datasets or unsorted data        |
| Binary Search | O(log n)        | Large datasets with sorted data        |

### 🧐 Which is More Suitable?

- **Binary Search** is more suitable when the product list is **large and pre-sorted**.
- **Linear Search** is suitable for **small or dynamic lists** where sorting isn’t required.


