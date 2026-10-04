# 🚀 SLE-3: Graph Search & Profiling Engine (BFS vs DFS)

---

## 📌 Project Overview

The **Graph Search & Profiling Engine** is a Python-based system designed to compare the performance of two classical uninformed search algorithms: **Breadth-First Search (BFS)** and **Depth-First Search (DFS)**.

The system operates on a binary-tree graph containing **65,535 vertices and 65,534 edges**, with Start Node `0` and Goal Node `30,000`. It measures execution time and nodes expanded to analyze the performance of both algorithms.

The architectural design follows the **Full C4 Software Architecture Model (Levels 1–4)** to ensure modularity, clarity, and separation of responsibilities.

---

## 🏗️ Architectural Design (Full C4 Model)

The system architecture is represented using four levels of the C4 Model.

### 📍 Level 1: System Context Diagram

Defines the system boundary and interaction between the external User/Operator and the Graph Search & Profiling Engine.

![Level 1 Context Diagram](./diagrams/C4_Level_1_Context.png)

* **Input Parameters:** Graph size (`65,535`), Start Node (`0`), Goal Node (`30,000`), and algorithm selection.
* **Core Processing:** Executes BFS or DFS and tracks node traversal.
* **Output Deliverables:** Search results, execution time, and nodes expanded.

---

### 📍 Level 2: Container Diagram

Represents the internal architecture by dividing the system into six functional modules.

![Level 2 Container Diagram](./diagrams/C4_Level_2_Container.png)

1. **Input & Configuration Module:** Accepts graph parameters and algorithm selection.
2. **Graph Generator:** Creates the binary-tree graph structure.
3. **Search Engine Core:** Executes BFS and DFS traversal algorithms.
4. **Frontier & Traversal Memory:** Manages the queue, stack, and visited nodes.
5. **Performance Profiler:** Measures execution time and nodes expanded.
6. **Output & Report Module:** Displays search results and performance comparisons.

---

### 📍 Level 3: Component Diagram

Zooms inside the **Search Engine Core** container to illustrate its internal components and relationships.

![Level 3 Component Diagram](./diagrams/C4_Level_3_Component.png)

* **Search Controller:** Manages the execution flow of the selected algorithm.
* **BFS Search Component:** Performs level-by-level traversal using a queue.
* **DFS Search Component:** Explores nodes deeply using a stack.
* **Frontier Manager:** Handles the data structure used for traversal.
* **Visited Node Tracker:** Maintains records of explored nodes.
* **Goal Test:** Checks whether the current node matches the target node.

---

### 📍 Level 4: Code / Class Diagram

Provides a detailed representation of the main functions, classes, and data structures used in the implementation.

![Level 4 Code Diagram](./diagrams/C4_Level_4_Code.png)

* `Graph`: Stores the graph structure.
* `bfs()`: Implements Breadth-First Search.
* `dfs()`: Implements Depth-First Search.
* `visited`: Tracks explored nodes.
* `goal_test()`: Checks the target node.
* `profiler`: Measures execution performance.
* `main()`: Controls program execution.

---

## 📊 Performance Benchmarking Metrics

| Metric           | BFS            | DFS                   |
| ---------------- | -------------- | --------------------- |
| Data Structure   | Queue (FIFO)   | Stack (LIFO)          |
| Search Strategy  | Level-by-Level | Deep-Path Exploration |
| Execution Time   | 4.53 ms        | 22.33 ms              |
| Nodes Expanded   | 15,000         | 54,472                |
| Time Complexity  | O(V + E)       | O(V + E)              |
| Space Complexity | O(V)           | O(V)                  |

*Note: Performance values are from the reported experiment. Verify them against your actual implementation before submission.*

---

## 🔑 Key Technical Design Decisions

* **Modular Architecture:** Separates graph generation, searching, profiling, and reporting.
* **Efficient Data Structures:** Uses a queue for BFS and a stack for DFS.
* **Performance Monitoring:** Measures execution time and nodes expanded.
* **Separation of Concerns:** Keeps search logic independent from performance measurement.
* **C4 Standardization:** Represents the system through Context, Container, Component, and Code diagrams.

---

## 🛠️ How to Run

### Step 1: Clone the Repository

```bash
git clone YOUR_REPOSITORY_URL
```

### Step 2: Navigate to Project Directory

```bash
cd IAI-SLE3-25UME044
```

### Step 3: Execute the Program

```bash
python main.py
```

---

## 🎯 Project Objectives

* Implement BFS and DFS algorithms.
* Perform searching on a binary-tree graph.
* Analyze execution time and nodes expanded.
* Compare the performance of both algorithms.
* Represent the architecture using the Full C4 Model.

---

## 📝 Conclusion

The project demonstrates the implementation and performance comparison of BFS and DFS algorithms. The Full C4 Model provides a structured representation of the system architecture, improving clarity, modularity, and maintainability.

---

## 👨‍💻 Student Details

* **Name:** Ganesh Ujesh Raut
* **PRN:** 25UME044
* **Division:** A
* **Department:** Artificial Intelligence and Machine Learning
* **Institute:** DKTE Society's Textile and Engineering Institute, Ichalkaranji
* **Subject:** Introduction to Artificial Intelligence
* **Course Code:** 02AML204
* **Activity:** SLE-3 – Architectural Design using Full C4 Model
* **Academic Year:** 2026–2027

---

## 🤖 AI Contribution

ChatGPT was used as a learning assistant for understanding algorithms, architectural design, and documentation. Implementation, execution, and verification were performed by the student.
