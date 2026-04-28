# HPC-Project-Parallel-Backtracking-Solver

🚀 Parallel Backtracking Algorithms — HPC Project
📌 Overview

This project demonstrates the use of parallel backtracking algorithms to solve computationally intensive problems using High Performance Computing (HPC) concepts.

The following problems are implemented:

👑 N-Queens Problem
🔢 Sudoku Solver
🧭 Traveling Salesman Problem (TSP)

Each problem is solved using both serial and parallel approaches to compare performance.

⚙️ Parallelization Strategy

| Problem  | Strategy                                                 |
| -------- | -------------------------------------------------------- |
| N-Queens | Each thread explores a different column in the first row |
| Sudoku   | Threads try different values for the first empty cell    |
| TSP      | Each thread starts from a different next city            |

🛠️ Technologies Used
C Programming
OpenMP (Parallel Computing)
GCC Compiler

🚀 Features
Parallel implementation using multi-threading
Efficient backtracking algorithms
Performance comparison between serial and parallel execution
Scalable for larger problem sizes

📊 Performance Insight
Parallel execution significantly reduces computation time by exploring multiple branches of the search space simultaneously.

▶️ How to Run
Step 1: Compile

gcc -fopenmp nqueens.c -o nqueens
gcc -fopenmp sudoku.c -o sudoku
gcc -fopenmp tsp.c -o tsp

Step 2: Run

OMP_NUM_THREADS=4 ./nqueens
OMP_NUM_THREADS=4 ./sudoku
OMP_NUM_THREADS=4 ./tsp

🧠 Key Concepts
Backtracking Algorithms
Parallel Computing
Multi-threading (OpenMP)
Constraint Satisfaction Problems

🎯 Learning Outcomes
Improved understanding of parallelizing recursive algorithms
Learned how to divide search space across threads
Gained experience in optimizing performance using HPC techniques


📁 Project Structure
.
├── nqueens.c
├── sudoku.c
├── tsp.c
└── README.md

💡 Future Improvements
Add visualization for solutions
Extend to GPU-based parallelism (CUDA)
Optimize load balancing between threads


