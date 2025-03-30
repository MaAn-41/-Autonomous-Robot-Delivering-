# Grid-Based Delivery Simulation using A* and BFS

## Overview
This project implements a **grid-based navigation and delivery system** using **Pygame**. It features an **autonomous robot** that navigates a **15x15 grid** to deliver items to designated locations while avoiding obstacles. The robot employs **A* Search Algorithm and Best-First Search (BFS)** to determine the most optimal path to its goal.

## Features
- **Pathfinding Algorithms:** Implements A* Search and Best-First Search for optimal path selection.
- **Dynamic Obstacles:** Houses, cars, and ambulances serve as obstacles.
- **Randomized Cost Generation:** Each grid cell has a randomly assigned traversal cost.
- **Item Delivery System:** Users can select items for delivery.
- **Interactive UI:** Uses Pygame for rendering the grid, obstacles, and interactive elements.
- **Performance Metrics:** Tracks time and space complexity for algorithm efficiency comparison.

## Installation
### Prerequisites
Ensure you have **Python 3.x** installed along with the required dependencies:

```sh
pip install pygame
```

### Clone the Repository
```sh
git clone https://github.com/MaAn-41/-Autonomous-Robot-Delivering-.git
cd grid-delivery-simulation
```

## Usage
Run the main script to start the simulation:
```sh
python main.py
```

### Controls & Interaction
- Click on item buttons to select items for delivery.
- Delivery locations are generated dynamically.
- The robot autonomously navigates towards the delivery point.
- The system compares **A* Search and BFS**, selecting the more efficient approach.

## Pathfinding Algorithms
### 1. A* Search
- Uses **G(n) + H(n)** where:
  - `G(n)` = cost from the start node to the current node.
  - `H(n)` = heuristic cost from the current node to the goal.
- Provides an optimal path considering traversal costs.

### 2. Best-First Search (BFS)
- Explores the lowest-cost neighbor first.
- May not always find the optimal path but is computationally efficient.

## Performance Comparison
The system dynamically selects the more efficient algorithm by comparing **time complexity** and **space complexity** for A* and BFS.

## File Structure
```
├── assets/                   # Images for houses, robot, cars, ambulance, and items
├── main.py                   # Main script to run the simulation
├── pathfinding.py            # A* and BFS implementations
├── utils.py                  # Helper functions for grid operations
├── README.md                 # Documentation
```

## Future Enhancements
- Implement **Dijkstra’s Algorithm** for an alternative pathfinding method.
- Enhance UI with a **dashboard** displaying algorithm performance in real-time.
- Introduce **dynamic obstacles** that move over time.

## License
This project is licensed under the **MIT License**.

---
📌 **Author:** M. Usman Aziz  
📧 Contact: usmanamjad495@gmail.com  
🔗 GitHub: [your-repo](https://github.com/MaAn-41/-Autonomous-Robot-Delivering-.git)

