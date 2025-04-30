# TSP Solver and Optimization
## Project Overview
This project is designed to solve the Traveling Salesman Problem (TSP) using a combination of Christofides' algorithm (or other heuristics) and optimization techniques such as simulated annealing. The solution is further optimized using local search methods, particularly the 2-opt exchange method, to minimize the total travel distance. The project handles clusters of locations, computes the TSP route for each cluster, and applies simulated annealing to improve the solution.

## Key Features

TSP Solver: Implements a solution for the Traveling Salesman Problem using heuristic methods (e.g., Christofides' algorithm).

Optimization: Applies simulated annealing to optimize the initial TSP solution.

2- opt Local Search: Uses a 2-opt exchange method to improve the route further.

## Project Structure


├── README.md                  # Project documentation
├── main_lab.ipynb             # Main lab for preparing the generated data and solving TSP using heuristic algorithms .
├──data/
        ├──Data_Generator.ipynb # contains scripts to generate the random graph vertices and cost matrix to get fed to the main lab     

## Description of Files:
main: This cell handles the overall execution of the program. It iterates over multiple clusters of locations, solves the TSP for each cluster, and applies optimization techniques.

tss_solver: Contains the implementation of the Traveling Salesman Problem solver using heuristics such as Christofides' algorithm. It also defines the search class used for TSP solving.

optimizors_v2: Implements the simulated annealing and 2-opt optimization techniques to refine the TSP solution.

clusters_data: Holds the location data and the associated edges and vertices for each cluster.

utils: Includes helper functions for calculating distances between points and other necessary utilities.

visualization: Contains the logic for live visualizing the TSP route evolution using matplotlib and animation.

## Installation
To run the TSP solver, you need Python 3.x installed. You can install the necessary dependencies by following the steps below:

## Clone the repository:
```
git clone https://github.com/yourusername/TSP_Solver_Project.git
cd TSP_Solver_Project
Create a virtual environment (optional but recommended):
```
```
python3 -m venv venv
source venv/bin/activate  # For Linux/Mac
venv\Scripts\activate     # For Windows
Install the required dependencies:
```
```
pip install -r requirements.txt
```
## Usage

To run the TSP solver on a specific cluster of locations, you can follow instruction within the main notebook.

Dependencies
numpy: For mathematical operations.

pandas: For handling and processing location data.

matplotlib: For plotting and visualization.

scipy: For additional mathematical tools.

networkx: For graph-related computations and TSP-solving logic.

random: For random number generation (used in optimization).

datetime: For timing execution.

To install the required dependencies, run:

bash
Copy
Edit
pip install -r requirements.txt
