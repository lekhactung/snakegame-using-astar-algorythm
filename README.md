# Snake Game Using A* Algorithm

## Introduce
This project simulates the Snake game. 

The special feature is instead of being controlled by a player, the snake 
is automatically controlled using the A* algorithm to find the shortest path to the food.

---

## Requirements
- Python 
- Libary:
  - `pygame`
install by:
```bash
    pip install pygame
```
---
## How to use
```bash
    python snakegame_using_astar.py
```
---
## How this works

The snake starts at the top-left corner of the screen.

Each time food appears, the agent uses the A* algorithm to calculate 
the shortest path from the snake’s head to the food while avoiding collisions with its own body.

If there is no valid path left → game over.

When the snake eats food, it grows longer and the score increases.

---
## A* algorithm
A* (A Star) is a computer algorithm that is widely used in 
pathfinding and graph traversal. The algorithm efficiently plots a walkable path between multiple nodes, or points, on the graph

A* expands paths that are already less expensive by using this function:
```bash
    f(n) = g(n) + h(n)  
```
- f(n) = total estimated cost of path through node n
- g(n) = cost so far to reach node n
- h(n) = estimated cost from n to goal. This is the heuristic part of the cost function
- this case using Manhattan distance for heuristic

The A* algorithm guarantees finding the shortest path (if one exists).

---
## Demo
![Demo](./assets/snakegame_demo_run.gif)
---
## 🔗 References
- This project is built based on the Snake Game from the project by **rajatdiptabiswas**.
- Repo URL : https://github.com/rajatdiptabiswas/snake-pygame/tree/master
---
