#Numerical Analysis of Volterra Delay Differential Equations

Convergence and Error Study using Collocation-Based Methods

📌 Overview

This project develops and analyzes numerical methods for solving Volterra delay differential and integral equations. The focus is on convergence analysis, stability properties, and systematic error evaluation across different test cases.

⚙️ Methodology

- Constructed a collocation-based numerical scheme using quadrature nodes and weights
- Designed interpolation basis functions for solution approximation
- Incorporated delay terms using fractional indexing and decomposition techniques
- Implemented iterative solvers for nonlinear systems at each discretized time step

🧠 Mathematical Framework

The approach is based on:

- Volterra delay differential and integral equations
- Collocation and quadrature methods
- Stability and convergence theory
- Error estimation techniques

💻 Implementation

- Implemented in Wolfram Mathematica
- Developed algorithms for time discretization and numerical approximation
- Handled delay terms using floor-based indexing and interpolation
- Solved nonlinear systems iteratively at each step

📊 Numerical Results

Two benchmark problems were studied with known exact solutions:

Example 1:

- Exact solution: y(t) = \sin(t)
- Tested for different delay parameters (q = 0.5, 0.33, 0.25)
- Observed decreasing error as the number of grid points increased
- Maximum error reached approximately 10^{-4}

Example 2:

- Exact solution: y(t) = \cosh(t)
- Evaluated under multiple discretization levels
- Achieved high accuracy with errors on the order of 10^{-5}

📈 Key Findings

- The numerical method demonstrates clear convergence behavior
- Error decreases consistently with finer discretization
- The approach remains stable across different delay parameters and kernel functions
- The method is robust for both trigonometric and exponential-type solutions

🚀 Relevance to Artificial Intelligence

This work is closely related to:

- Numerical optimization techniques used in machine learning
- Dynamical systems modeling in AI
- Stability and convergence analysis in iterative algorithms
- Computational methods for data-driven modeling

🔗 Author

Shiva Karimi
