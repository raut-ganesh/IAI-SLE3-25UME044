Graph Search & Profiling Engine

BFS vs DFS Performance Profiling

A Python-based Artificial Intelligence project that implements and compares Breadth-First Search (BFS) and Depth-First Search (DFS) on a large binary-tree graph.

The project focuses on measuring and analyzing execution time and nodes expanded during graph traversal.

---

📌 Overview

The Graph Search & Profiling Engine performs graph searching using two classical AI search algorithms:

- BFS (Breadth-First Search) — explores nodes level by level using a queue.
- DFS (Depth-First Search) — explores nodes deeply using a stack.

The system records the performance of both algorithms and provides a comparison based on the experimental results.

---

🎯 Objectives

- Implement BFS and DFS in Python.
- Generate and search a large binary-tree graph.
- Track the number of nodes expanded.
- Measure algorithm execution time.
- Compare BFS and DFS performance.
- Understand the practical behavior of AI search algorithms.

---

🌳 Graph Configuration

Parameter| Value
Graph Type| Binary Tree
Number of Vertices| 65,535
Number of Edges| 65,534
Search Algorithms| BFS & DFS
Language| Python

---

🔎 Algorithms

Breadth-First Search — BFS

BFS explores the graph level by level using a queue.

Main characteristics:

- Queue-based traversal
- Level-wise exploration
- Suitable for finding the shortest path in an unweighted graph

Depth-First Search — DFS

DFS explores a branch as deeply as possible before backtracking.

Main characteristics:

- Stack-based traversal
- Depth-wise exploration
- Useful for exploring deep graph structures

---

📊 Experimental Results

The selected SLE-2 experiment produced the following results:

Metric| BFS| DFS
Average Execution Time| 4.53 ms| 22.33 ms
Nodes Expanded| 15,000| 54,472

Result Analysis

In the selected experiment, BFS recorded lower execution time and fewer nodes expanded than DFS.

These results are specific to the tested graph, goal node, implementation, and execution environment. They should not be interpreted as meaning that BFS is always faster than DFS.

---

🏗️ Architecture — C4 Model

The system architecture is represented using the C4 Model.

Level 1 — Context

Shows the interaction between the User/Operator, Graph Search & Profiling Engine, and Performance Report.

Level 2 — Containers

The system is divided into six logical containers:

1. Input & Configuration Module
2. Graph Generator
3. Search Engine Core
4. Frontier & Traversal Memory
5. Performance Profiler
6. Output & Report Module

Level 3 — Components

The Search Engine Core contains:

- Search Controller
- BFS Search Component
- DFS Search Component
- Frontier Manager
- Visited Node Tracker
- Goal Test & Search Result

Level 4 — Code Level

The main implementation elements include:

graph
 └── Stores the graph using an adjacency structure

bfs()
 └── Performs Breadth-First Search

dfs()
 └── Performs Depth-First Search

visited
 └── Tracks explored nodes

nodes_expanded
 └── Counts examined nodes

goal_test()
 └── Checks the target node

Performance Profiler
 └── Measures execution time and profiling information

main()
 └── Executes the experiment and displays results

«The code-level names should match the actual implementation in the repository.»

---

🛠️ Technologies Used

- Python
- NetworkX
- Matplotlib
- timeit
- Python data structures such as Queue, Stack, and Set

---

📂 Project Structure

Graph-Search-Profiling/
│
├── sle2_bfs_vs_dfs.py
├── AI Contribution log.md
├── README.md
└── images/
    └── architecture/

---

▶️ How to Run

Clone the Repository

git clone YOUR_REPOSITORY_LINK

Navigate to the Project

cd Graph-Search-Profiling

Install Dependencies

pip install networkx matplotlib

Run the Program

python sle2_bfs_vs_dfs.py

---

📚 Learning Outcomes

This project helped me understand:

- BFS and DFS search strategies
- Queue- and stack-based traversal
- Graph representation using adjacency structures
- Visited-node tracking
- Performance profiling
- Algorithm comparison
- C4 software architecture
- Modular system design

---

🤖 AI Contribution

AI Tool Used: ChatGPT

AI assistance was used for understanding the C4 architecture model, organizing architectural levels, preparing diagram layouts, and improving technical explanations.

The program was executed and tested, the BFS and DFS results were reviewed, and the final project architecture and documentation were prepared and verified by the student.

---

👨‍💻 Author

Ganesh Ujesh Raut

PRN: 25UME044
Division: A
Course: 02AML204 – Introduction to Artificial Intelligence
Department: CSE (AIML)
Institute: D.K.T.E. Society's Textile and Engineering Institute, Ichalkaranji

---

🎓 Academic Project

Developed as part of the SLE-2 Performance Profiling and SLE-3 Architectural Design activities for:

02AML204 — Introduction to Artificial Intelligence
