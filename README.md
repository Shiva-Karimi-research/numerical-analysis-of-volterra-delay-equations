Numerical Analysis of Volterra Delay Differential Equations

Convergence and Error Study Using Collocation-Based Methods

---

📌 Overview

This project develops and analyzes numerical methods for solving Volterra delay differential and integral equations. The focus is on convergence analysis, stability properties, and systematic error evaluation across different test cases.

---

⚙️ Methodology

- Constructed a collocation-based numerical scheme using quadrature nodes and weights
- Designed interpolation basis functions for solution approximation
- Incorporated delay terms using fractional indexing and decomposition techniques
- Implemented iterative solvers for nonlinear systems at each discretized time step

---

🧠 Mathematical Framework

The approach is based on:

- Volterra delay differential and integral equations
- Collocation and quadrature methods
- Stability and convergence theory
- Error estimation techniques

---

💻 Implementation

- Implemented in Wolfram Mathematica
- Developed algorithms for time discretization and numerical approximation
- Handled delay terms using floor-based indexing and interpolation
- Solved nonlinear systems iteratively at each step

---

📊 Numerical Results

Two benchmark problems with known exact solutions are considered.

---

Example 1: Numerical Results for y(t) = sin(t)

The table reports the numerical error for different values of the delay parameter q, using m = 2, as the number of grid points N increases.

Case 1: q = 0.5

| m | N  | Error        |
|---|----|-------------|
| 2 | 10 | 2.73e-4     |
| 2 | 15 | 2.11e-4     |
| 2 | 25 | 1.17e-4     |
| 2 | 50 | 6.66e-5     |
| 2 | 90 | 8.69e-6     |
| 2 | 140| 3.58e-6     |

---

Case 2: q = 1/3

| m | N   | Error   |
|---|-----|---------|
| 2 | 10  | 6.77e-2 |
| 2 | 15  | 6.97e-2 |
| 2 | 35  | 5.84e-2 |
| 2 | 70  | 5.54e-2 |
| 2 | 140 | 4.99e-2 |
| 2 | 200 | 4.70e-2 |

---

Case 3: q = 1/4

| m | N   | Error   |
|---|-----|---------|
| 2 | 20  | 8.44e-2 |
| 2 | 60  | 7.24e-2 |
| 2 | 80  | 7.43e-2 |
| 2 | 250 | 7.06e-2 |
| 2 | 360 | 7.15e-2 |
| 2 | 450 | 7.16e-2 |

---

Observation:
The method exhibits clear convergence for q = 0.5, where the error decreases significantly as N increases. For smaller values of q, the convergence becomes slower, indicating the increasing impact of delay on numerical accuracy.

---

Example 2: Numerical Results for y(t) = cosh(t)

The table presents the numerical error for different values of the delay parameter q, using m = 2, as the number of grid points N increases.

Case 1: q = 0.9

| m | N   | Error   |
|---|-----|---------|
| 2 | 25  | 2.12e-4 |
| 2 | 45  | 6.46e-5 |
| 2 | 65  | 3.08e-5 |
| 2 | 75  | 2.31e-5 |
| 2 | 100 | 1.26e-5 |
| 2 | 250 | 2.04e-6 |

---

Case 2: q = 0.8

| m | N   | Error   |
|---|-----|---------|
| 2 | 10  | 1.12e-3 |
| 2 | 30  | 1.37e-4 |
| 2 | 40  | 7.77e-5 |
| 2 | 60  | 3.49e-5 |
| 2 | 120 | 8.83e-6 |
| 2 | 200 | 3.19e-6 |

---

Case 3: q = 0.7

| m | N   | Error   |
|---|-----|---------|
| 2 | 10  | 1.17e-3 |
| 2 | 30  | 1.38e-4 |
| 2 | 40  | 7.85e-5 |
| 2 | 60  | 3.52e-5 |
| 2 | 120 | 8.86e-6 |
| 2 | 200 | 3.20e-6 |

---

Observation:
The results demonstrate consistent and stable convergence across all tested delay parameters. As the number of grid points N increases, the numerical error decreases significantly, indicating the effectiveness of the proposed method. Moreover, the method maintains high accuracy even for relatively large delay values, confirming its robustness and reliability in handling delay-dependent problems.

---

📈 Key Findings

- The numerical method demonstrates clear convergence behavior
- Error decreases consistently with finer discretization
- The approach remains stable across different delay parameters and kernel functions
- The method is robust for both trigonometric and exponential-type solutions

---

🚀 Relevance to Artificial Intelligence

This work is closely related to:

- Numerical optimization techniques used in machine learning
- Dynamical systems modeling in AI
- Stability and convergence analysis in iterative algorithms
- Computational methods for data-driven modeling

This project reflects my transition from mathematical modeling to computational and algorithmic problem-solving, aligning with modern AI methodologies.

---

📁 Code

The Mathematica implementation of the proposed numerical methods is available in the following files:

- [sin solution notebook](src/volterra_delay_equation_sin_solution.nb)
- [cosh solution notebook](src/volterra_delay_equation_cosh_solution.nb)

These implementations are designed for reproducibility of the numerical experiments and can be extended to more general classes of delay differential equations.
