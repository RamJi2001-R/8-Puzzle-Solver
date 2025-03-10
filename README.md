# 8-Puzzle-Solver

## Description
This project implements an **8-Puzzle Solver** using the **A* (A-Star) Algorithm** in Python. The A* algorithm efficiently finds the optimal solution by utilizing the **Manhattan Distance** heuristic.

## Features
- Uses **A* Search Algorithm** for solving the 8-puzzle.
- Implements **Manhattan Distance** heuristic to estimate cost.
- Keeps track of the **solution path** from the initial state to the goal state.
- Prints each step required to solve the puzzle.

## Requirements
This project requires **Python 3.x**. No external libraries are needed as it only uses the built-in `queue.PriorityQueue` for priority-based state expansion.

## Installation
Clone the repository and navigate to the project folder:
```sh
 git clone https://github.com/your-username/8-puzzle-solver.git
 cd 8-puzzle-solver
```

## How to Run
1. Ensure you have **Python 3.x** installed.
2. Run the script using the following command:
   ```sh
   python 8_puzzle_solver.py
   ```
3. The program will output the steps to reach the goal state.

## Example Input
The initial puzzle state is predefined in the script:
```python
initial_board = [
    [1, 2, 3],
    [4, 0, 6],
    [7, 5, 8]
]
```

## Example Output
```
Solution found!
Step 0: Move 
[1, 2, 3]
[4, 0, 6]
[7, 5, 8]

Step 1: Move DOWN
[1, 2, 3]
[4, 5, 6]
[7, 0, 8]

Step 2: Move RIGHT
[1, 2, 3]
[4, 5, 6]
[7, 8, 0]
```

## Algorithm Explanation
The **A* algorithm** is used to find the shortest path to the goal state:
- **g(n):** Cost to reach the current state.
- **h(n):** Estimated cost to reach the goal (Manhattan Distance heuristic).
- **f(n) = g(n) + h(n):** Total estimated cost.

The algorithm explores states in order of increasing cost, ensuring the shortest path is found efficiently.

## Contributing
Contributions are welcome! Feel free to fork this repository, make improvements, and submit a pull request.

## License
This project is open-source and can be modified or distributed freely.

## Author
[Your Name]

## Repository
[GitHub Repository](https://github.com/your-username/8-puzzle-solver)

