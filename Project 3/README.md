# Project 3: PageRank Algorithm Implementation

## Overview

This project involves the implementation and analysis of the PageRank algorithm, a key algorithm used by search engines to rank web pages. The notebook includes the following major steps:

1. **Data Loading**: Reads a dataset and initializes the adjacency matrix using sparse matrix representation.
2. **Power Iteration Implementation**: Defines and executes the power iteration method to compute the PageRank scores.
3. **Top-10 List Generation**: Extracts and displays the top-10 nodes based on their PageRank scores.
4. **Extended PageRank Function**: Implements an extended version of the PageRank algorithm, incorporating a teleportation factor (damping factor).
5. **Visualization**: Plots various graphs to visualize the convergence and the effect of the damping factor on the number of iterations required.

## Key Components

### Data Loading
- Reads the dataset from a file (`web-Google.txt`).
- Initializes the adjacency matrix `M` using `csc_matrix` from `scipy.sparse`.

### Power Iteration Algorithm
- Defines the `power_iteration` function to compute the PageRank scores.
- This function iteratively updates the rank vector until the change between iterations falls below a specified threshold.
- Calculates and stores the "leaked score" at each iteration.

### Top-10 List Generation
- Defines a function to generate and display the top-10 nodes based on their PageRank scores.

### Extended PageRank Algorithm
- Implements an extended version of the PageRank algorithm to include the teleportation factor (damping factor).
- Ensures the sum of PageRank scores remains 1 by adjusting for the damping factor.

### Visualization
- Plots the leaked scores over iterations to visualize the convergence of the power iteration method.
- Plots the number of iterations required for different beta values to observe the effect of the damping factor on convergence speed.

## Running the Project
1. **Load the Data**: Read the dataset and initialize the adjacency matrix.
2. **Execute Power Iteration**: Run the `power_iteration` function to compute the PageRank scores and capture the runtime and number of iterations.
3. **Generate Top-10 List**: Use the top-10 function to extract and display the top-10 nodes.
4. **Run Extended PageRank**: Execute the `PageRank` function with different beta values and capture the runtime and number of iterations.
5. **Visualize Results**: Plot the leaked scores and the number of iterations required for different beta values.

## Key Insights
- The power iteration method effectively computes the PageRank scores, and the convergence can be visualized by plotting the leaked scores over iterations.
- The damping factor (beta) significantly affects the number of iterations required for convergence, which can be observed by plotting iterations against different beta values.

## Conclusion
This project provides a comprehensive implementation and analysis of the PageRank algorithm using the power iteration method. The extended PageRank function with a damping factor ensures more accurate and realistic computation of PageRank scores, and the visualizations offer insights into the convergence behavior of the algorithm.
