# 🧠 Q-Learning for Shortest Path Finding

This repository implements a reinforcement learning solution to the shortest path problem using the Q-learning algorithm. The environment is a 4x4 grid transformed into a graph where each cell represents a node, and each movement corresponds to a graph edge. Some edges are marked as **broken arcs** (impassable), making the environment partially constrained.

## 🔍 Problem Setting
- Grid world is modeled as an undirected graph `G(N, A)`.
- Certain edges are considered "broken", i.e., inaccessible with heavy negative rewards.
- The agent starts at node `0` and must reach the target node `15`.
- Broken arcs are hard-penalized with rewards of `-100`.
- Arcs leading directly to the target receive `+100`.
- All other transitions receive neutral rewards (`0`).

## 🧠 Solution: Q-Learning
- Initialized Q-table for all state-action pairs.
- Applied ε-greedy strategy for balancing exploration and exploitation.
- Updated Q-values using the Bellman equation.
- Trained over multiple episodes until convergence.

## 📊 Visualization
The learned optimal path is visualized on a grid with:
- 🔵 Start node
- 🔴 Goal node
- 🟩 Traversable nodes
- 🚫 Broken arcs

## 🛠 Tools & Libraries
- Python
- NumPy
- NetworkX
- Matplotlib
- Jupyter Notebook

## 🚀 Run It
Simply run the notebook step-by-step. All dependencies are standard Python libraries.

## 📎 License
MIT

## 👨‍🔬 Author
Reza Mirjalili – PhD Candidate in Operations Research  
University of Houston | [LinkedIn](https://linkedin.com/in/rezamirjaliliphd)
