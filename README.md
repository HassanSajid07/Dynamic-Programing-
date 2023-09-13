# Dynamic-Programing-
Markov decision process
This C++ code is a simulation program that computes and optimizes a policy for a dynamic decision-making problem in a grid-based environment. The code uses a Markov Decision Process (MDP) framework to model the problem. Here's a brief description of its main components and functionalities:

    Header Includes and Definitions: The code includes necessary header files, defines macros for minimum and maximum, and sets various constants related to grid dimensions, time, and other parameters.

    Global Variables: It declares global multidimensional arrays to store probabilities, rewards, policies, allowances, and travel times. It also initializes a memoization table to store computed values for optimization.

    Initialization: The initialize function reads data from external CSV files to populate the arrays with probabilistic information about finding destinations, allowances, destination probabilities, rewards, and travel times.

    Utility Functions: Several utility functions are defined, such as check, extractValue, newx, newy, is_allowed, and others, to perform calculations and checks related to grid movement and value extraction.

    Value Iteration: The core of the program is the V function, which implements the value iteration algorithm. It computes the expected rewards for different actions in each state and time step, updating the memoization table for efficient computation.

    Main Function: The main function controls the overall flow of the program. It initializes random numbers, calls the initialize function to load data, and performs value iteration to optimize policies for each grid cell and time step.

    Output: The code prints the computed policies and values for each time step and grid cell. It also outputs this data to CSV files for further analysis.
