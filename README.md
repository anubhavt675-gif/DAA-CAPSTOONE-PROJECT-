# SMART COURIER: Intelligent Parcel Packing & Route Optimization System

> **B.Tech Design and Analysis of Algorithms (DAA) Capstone Project**  
> A complete, working Python application integrating Sorting Algorithms, Dynamic Programming, Graph Algorithms, Shortest Path Algorithms, TSP Approximation Techniques, and Empirical Runtime Analysis.

---

## 1. Problem Statement

Modern logistics and courier companies face two fundamental computational challenges daily:

1. **Parcel Prioritization & Selection (Packing Problem):** With hundreds of parcels possessing distinct deadlines, priority tiers, weights, and values, which optimal subset should be loaded into a vehicle with strict weight capacity limits to maximize total delivered value?
2. **Delivery Route Optimization (Routing Problem):** In what optimal sequence should delivery destinations be visited to minimize fuel consumption, driver travel time, and total transit distance before returning to the central distribution hub?

Both problems belong to classical computational complexity classes: the 0/1 Knapsack problem is NP-complete, and the Travelling Salesman Problem (TSP) is NP-hard. This application provides real, non-trivial, and mathematically rigorous algorithmic solutions executed dynamically on real input datasets.

---

## 2. Project Objectives

- **Algorithmic Correctness:** Implement pure algorithmic implementations from scratch without external black-box algorithm libraries.
- **End-to-End Modular Integration:** Connect parcel sorting, knapsack selection, shortest path extraction, and TSP routing into a single interactive terminal application.
- **Empirical Scalability Benchmarking:** Rigorously test and measure algorithm runtimes across Small (15 items), Medium (150 items), and Large (700 items) datasets.
- **Academic Standard Documentation:** Provide formal time and space complexity evaluations, mathematical formulations, and visual performance charts for viva and presentation evaluation.

---

## 3. Features

- **Interactive Terminal Interface:** Clean, robust 11-option terminal menu with graceful input validation.
- **Stable 3-Tier Merge Sort:** Sorts parcels by earliest deadline $\rightarrow$ highest priority score $\rightarrow$ highest delivery value.
- **Bottom-Up 0/1 Knapsack Dynamic Programming:** Computes the global optimum without fractional packing, complete with 2D DP table construction and backtracking.
- **Dijkstra's Algorithm with Min-Heap Priority Queue:** Computes shortest road network paths ($O((V+E)\log V)$) using `heapq`, handling multi-hop road networks.
- **Nearest Neighbor TSP Approximation:** Computes an approximate closed-loop delivery tour returning to the depot.
- **Automated Performance Benchmarking:** Computes median runtimes across repeated trials, saving results to CSV and structured text reports.
- **High-Resolution Visualizations:** Matplotlib charts illustrating runtime scaling and comparative performance.
- **Automated Comprehensive Reporting:** Detailed dispatch manifests containing packed parcels, rejected items, vehicle utilization, step-by-step route legs, and runtime breakdowns.

---

## 4. Technologies Used

| Category | Technology | Usage |
|---|---|---|
| **Programming Language** | Python 3.10+ | Core application logic and algorithms |
| **Data Structures** | Custom / Built-in (`heapq`, lists, dicts) | Min-priority queues, graphs, DP tables |
| **Data Formats** | CSV & JSON | Parcel manifests and road network definitions |
| **Visualization** | Matplotlib (Agg backend) | Performance comparison charts |
| **Runtime Benchmarking**| `time.perf_counter()` | Sub-millisecond timing measurements |
| **Testing Framework** | `unittest` / `pytest` | 38 automated test cases |

---

## 5. System Architecture
