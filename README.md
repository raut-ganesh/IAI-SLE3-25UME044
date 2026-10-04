🔍 Graph Search & Profiling Engine

BFS vs DFS Performance Profiling

Author: Ganesh Ujesh Raut
PRN: 25UME044
Division: A
Department: CSE (AIML)
Course: 02AML204 — Introduction to Artificial Intelligence
Institute: D.K.T.E. Society's Textile and Engineering Institute, Ichalkaranji

---

«An AI-based graph search project for implementing, profiling, and comparing Breadth-First Search (BFS) and Depth-First Search (DFS).»

📌 Project Overview

The Graph Search & Profiling Engine is a Python-based system developed to study the practical performance of BFS and DFS on a large binary-tree graph.

The system executes both algorithms, tracks the number of nodes expanded, measures execution time, and compares their performance.

🎯 Objectives

- Implement BFS using a queue.
- Implement DFS using a stack.
- Generate a large binary-tree graph.
- Track expanded nodes.
- Measure execution time.
- Compare BFS and DFS performance.
- Design the system using the C4 Model.

🌳 Experiment Setup

Specification| Details
Graph Type| Binary Tree
Vertices| 65,535
Edges| 65,534
Algorithms| BFS & DFS
Language| Python

🧠 Algorithms

BFS — Breadth-First Search

BFS explores nodes level by level using a queue.

DFS — Depth-First Search

DFS explores one branch as deeply as possible using a stack before backtracking.

📊 Performance Results

SLE-2 Experimental Results

Metric| BFS| DFS
Average Execution Time| 4.53 ms| 22.33 ms
Nodes Expanded| 15,000| 54,472

Observation: In the selected experiment, BFS recorded lower execution time and fewer nodes expanded than DFS.

«Results depend on the graph structure, target node, implementation, and execution environment.»

🏗️ C4 Architecture

The project is represented using four C4 architectural levels.

Level 1 — Context

User / Operator
       │
       ▼
Graph Search & Profiling Engine
       │
       ▼
Performance Report

Level 2 — Containers

Input & Configuration
          ↓
     Graph Generator
          ↓
     Search Engine Core
          ↓
Frontier & Traversal Memory
          ↓
   Performance Profiler
          ↓
   Output & Report Module

Level 3 — Components

Search Engine Core

Search Controller
       │
   ┌───┴───┐
   ▼       ▼
  BFS     DFS
   │       │
   └───┬───┘
       ▼
Frontier Manager
       │
       ▼
Visited Node Tracker
       │
       ▼
Goal Test & Search Result

Level 4 — Code Overview

Element| Responsibility
"graph"| Stores graph using adjacency structure
"bfs()"| Performs Breadth-First Search
"dfs()"| Performs Depth-First Search
"visited"| Tracks explored nodes
"nodes_expanded"| Counts examined nodes
"goal_test()"| Checks the target node
"Performance Profiler"| Measures execution time
"main()"| Runs the experiment

«Code-level names should match the actual implementation.»

🛠️ Technologies Used

- Python
- NetworkX
- Matplotlib
- timeit
- Queue, Stack and Set data structures

📂 Project Structure

Graph-Search-Profiling/
│
├── 📄 sle2_bfs_vs_dfs.py
├── 📄 AI Contribution log.md
├── 📄 README.md
│
└── 📁 images/
    └── 📁 architecture/

▶️ How to Run

Clone the Repository

git clone YOUR_REPOSITORY_LINK

Install Dependencies

pip install networkx matplotlib

Run the Program

python sle2_bfs_vs_dfs.py

📚 Learning Outcomes

- Graph traversal algorithms
- BFS and DFS implementation
- Queue and stack-based searching
- Graph representation
- Node expansion tracking
- Performance profiling
- C4 software architecture
- Modular system design

🤖 AI Contribution

AI Tool Used: ChatGPT

AI assistance was used for understanding the C4 architecture model, organizing architectural levels, preparing diagram layouts, and improving technical documentation.

The program was executed and tested, the experimental results were reviewed, and the final implementation and documentation were verified by the student.

---

🎓 Academic Work

SLE-2: BFS vs DFS Performance Profiling
SLE-3: Architectural Design — Full C4 Model

---

⭐ Project Focus

Search → Profile → Compare → Analyze
