# Kruskal’s Algorithm — Minimum Spanning Tree (Python)

## 📌 Overview
This repository contains a clean and efficient Python implementation of
**Kruskal’s Algorithm** to compute the **Minimum Spanning Tree (MST)**
of a weighted, undirected graph.

The project focuses on:
- Algorithmic clarity
- Efficient cycle detection using **Union-Find**
- Readable and maintainable Python code

It is suitable for **learning**, **interview preparation**, and **DSA reference**.

---

## 🧠 What is a Minimum Spanning Tree (MST)?
Given a connected, weighted, undirected graph:
- A **spanning tree** connects all vertices without cycles
- A **minimum spanning tree** has the **lowest possible total edge weight**

An MST always contains:
- Exactly **V − 1 edges**
- No cycles
- Minimum total cost

---

## ⚙️ Algorithm Used: Kruskal’s Algorithm
Kruskal’s Algorithm is a **greedy algorithm** that builds the MST by selecting
edges in increasing order of weight.

### Steps:
1. Sort all edges by increasing weight
2. Pick the smallest edge
3. Add it to the MST **only if it does not form a cycle**
4. Repeat until **V − 1 edges** are selected

---

## 🧩 Cycle Detection: Union-Find (Disjoint Set)
To efficiently check whether adding an edge creates a cycle, the algorithm
uses the **Disjoint Set (Union-Find)** data structure.

### Optimizations Used:
- **Path Compression**: Flattens the structure during `find`
- **Union by Rank**: Keeps trees shallow for faster operations

These optimizations ensure near-constant time performance.

---
