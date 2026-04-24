# A* Heuristic Search Reproduction (CS5100 Final Project)

## Overview
This project reproduces and empirically evaluates the theoretical properties of the A* search algorithm by Hart, Nilsson, and Raphael (1968), with a focus on heuristic admissibility and its impact on optimality and computational efficiency.

The study investigates how different heuristic configurations affect A*'s behavior in practice across both uniform-cost and weighted-cost grid environments.

---

## Repository Structure

 - a_star_experiments.py: main implementation and experiment runner
 - analysis_and_plots.ipynb: Data analysis and visualization
 - figures directory: contains outputs (charts) of analysis_and_plots.ipynb

## How to Run

### Requirements
 - Python 3.x
 - No external dependendies required (standard libraries only)

### Run Experiments

Run the following command in terminal:
python3 astar_experiments.py

This will generate 20 valid grid layouts, run A* across multiple heuristics, and output average results for path cost, nodes expanded, and runtime.

Heuristics:
 - Zero (Dijkstra)
 - Manhattan distance
 - Weighted Manhattan heuristics (1.2, 2, 5, 10)

The Jupyter notebook runs the script and generates plots for path cost trends and node expansions.

All results are fully reproducible due to fixed random seeds.

## Reference
Hart, P., Nilsson, N., & Raphael, B. (1968). _A Formal Basis for the Heuristic Determination of Minimum Cost Paths_. IEEE Transactions on Systems Science and Cybernetics.
