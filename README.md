
# Artificial-Intelligence-Project

# N-Puzzle Solver

A Python-based N-Puzzle Solver with a **graphical user interface (GUI)** using Tkinter. This project allows users to input any N-Puzzle configuration, select a solving algorithm, and visualize the solution step by step.

---

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Supported Algorithms](#supported-algorithms)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Results](#results)
- [Author](#author)

---

## Overview

The N-Puzzle problem is a classic artificial intelligence problem where a board with sliding tiles must be arranged into a goal state. This project provides an interactive way to solve it using multiple search strategies and visualize the steps.

---

## Features

- GUI interface using **Tkinter**.
- Supports **dynamic puzzle size**: 2x2, 3x3, 4x4.
- Multiple search algorithms for solving:
  - Breadth First Search (BFS)
  - Depth First Search (DFS)
  - Uniform Cost Search (UCS)
  - Iterative Deepening
  - Depth Limited Search
  - A* Search
  - Greedy Best-First Search
- Step-by-step solution visualization.
- Displays solution metrics:
  - Time taken
  - Depth of solution (G-value)
  - Nodes processed
  - Maximum nodes stored
  - Moves sequence
- Input validation for correct puzzle states.

---

## Supported Algorithms

1. **Breadth First Search (BFS)**  
2. **Depth First Search (DFS)**  
3. **Uniform Cost Search (UCS)**  
4. **Depth Limited Search**  
5. **Iterative Deepening Search**  
6. **A* Search** (using Manhattan Distance heuristic)  
7. **Greedy Best-First Search** (using Manhattan Distance heuristic)  

---

## Installation

1. Make sure **Python 3.8+** is installed on your system.
2. Install required Python libraries:
```bash
pip install numpy
````

3. Clone this repository:

```bash
git clone <your-repo-link>
```

4. Navigate to the project directory:

```bash
cd N-Puzzle-Solver
```

---

## Usage

1. Run the application:

```bash
python project.py
```

2. In the GUI:

   * Select the **Puzzle Dimension** (2x2, 3x3, 4x4).
   * Click **Set Start State** and enter the initial configuration.
   * Click **Set Goal State** and enter the target configuration.
   * Select a **Solving Algorithm** from the dropdown menu.
   * Click **Solve Puzzle** to compute the solution.
   * Use **Next** and **Previous** buttons to navigate the solution step by step.
   * Click **Reset** to view the initial puzzle state again.

---

## How It Works

* Each puzzle configuration is represented as a **Node** containing:

  * `state` (board configuration)
  * `g` (cost or depth)
  * `parent` (previous node)
  * `action` (move taken)
* The **GoalTree** class manages the search process and builds the solution path.
* The solver explores puzzle states using the selected search algorithm until the goal state is reached.
* **Manhattan Distance heuristic** is used for A* and Greedy Best-First Search.
* The GUI updates dynamically to display each move visually.

---

## Results

After solving a puzzle, the GUI displays:

* **Time taken** to solve the puzzle.
* **Depth/level of the solution (G-value)**.
* **Number of nodes processed**.
* **Maximum nodes stored** in memory during search.
* **Whether the solution was found**.
* **Sequence of moves** required to reach the goal state.

---

## Author

**Muhammad Hamza Haroon**
Bachelor’s in Computer Science | NUCES FAST, Karachi, Pakistan
Junior Python & Web Developer

---
