# AutoRL-Zyara
Overview
This project implements a warehouse navigation system where an autonomous agent navigates from a starting position to a goal location while avoiding obstacles (shelves). The path is calculated using the A* algorithm, and further enhancements can be achieved using Deep Q-Network (DQN) and Particle Swarm Optimization (PSO) for more efficient navigation.
Features
A Algorithm: Computes the shortest path from the starting position to the destination while avoiding obstacles.
DQN Integration: Reinforcement learning technique to improve the agent's ability to navigate dynamically.
PSO Optimization: Used to optimize the path selection by reducing unnecessary movements.
Real-time Visualization: Uses Pygame to visually represent the warehouse, agent movement, and obstacles connect with 3d warehouse.

Technologies Used
Python
Pygame with unity (for visualization)
NumPy
TensorFlow/Keras (for DQN)
SciPy (for PSO optimization)

Installation
pip install pygame numpy tensorflow scipy
How to Run
Ensure the required libraries are installed.
Place the warehouse background image (3d_ware.jpg) in the same directory.


Run the script:
python warehouse_pathfinding.py
Input the desired product row and column.
The agent will move step-by-step towards the goal while avoiding obstacles.

A* Algorithm Implementation
Uses a priority queue (Min-Heap) to explore the lowest-cost path.
Calculates the heuristic using Manhattan distance.
Avoids obstacles by considering shelves as blocked cells.

DQN-Based Pathfinding Enhancement
The agent is trained using Deep Q-Learning to make better movement decisions.
The state space includes the grid position and possible moves.
The reward function penalizes obstacles and optimizes movement efficiency.
Implements an epsilon-greedy policy for action selection.

PSO-Based Path Optimization
Particles represent potential paths and evolve toward an optimal solution.
Uses a fitness function based on path length and collision avoidance.
Adjusts velocity and position of particles iteratively to find the best route.

Future Improvements
Implement dynamic obstacle detection and avoidance.
Optimize warehouse layout for efficient product retrieval.
Extend to multi-agent navigation scenarios.
