# Transportation-Problem-solver
Transportation Problem Solver (Python)

This repository contains a Python implementation of the classical Transportation Problem using standard Operations Research techniques.
The project supports both initial feasible solution methods and optimality testing using the MODI (u–v) method.

It is intended for engineering students, academic projects, and optimization studies related to logistics and supply chain management.

Key Features

Automatic balancing of unbalanced transportation problems

Support for multiple solution techniques

Modular, object-oriented implementation

Efficient matrix operations using NumPy

Suitable for academic and learning purposes

Methods Implemented

North-West Corner Rule (NWCR)
Generates a basic feasible solution without considering transportation cost.

Least Cost Method (LCM)
Allocates supply based on minimum transportation cost.

Vogel’s Approximation Method (VAM)
Uses penalty values to generate a near-optimal initial solution.

MODI Method (u–v Method)
Improves the initial solution iteratively to reach the optimal solution.

Problem Balancing

If total supply and total demand are unequal, the algorithm automatically:

Adds a dummy supply row or demand column

Assigns zero transportation cost to dummy allocations

This ensures that the problem remains solvable.

Usage Example
tp = TransportationProblem(cost_matrix, supply, demand)

initial_solution = tp.solve('VAM')
optimal_solution = tp.solve('MODI')

Applications

Operations Research coursework

Transportation and logistics optimization

Supply chain planning problems

Academic mini and major projects

Technologies Used

Python

NumPy

Pandas (optional, for extensions)
