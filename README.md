# Virtual Robot Navigation

## Overview

This project is a Python-based simulation of a robot navigating through a grid environment while avoiding obstacles and finding a route to a destination.

I created this project to explore the fundamentals of robotics path planning and algorithms without using physical hardware.

## Project Objectives

- Represent a robot's environment using a grid.
- Allow the robot to identify valid and blocked positions.
- Implement a pathfinding algorithm.
- Find a route from a starting position to a goal.
- Visualize the planned route.
- Test the algorithm with different obstacle layouts.

## How It Works

The environment is represented as a grid.

- `S` = starting position
- `G` = goal
- `#` = obstacle
- `.` = open space

The robot can move up, down, left, or right.

Before moving, the program checks whether the new position is inside the grid and whether the position contains an obstacle.

## Algorithm

The project uses **Breadth-First Search (BFS)** to find a route from the starting position to the goal.

BFS explores possible positions level by level. When every movement has the same cost, BFS can find a shortest route in terms of the number of moves.

## Tools Used

- Python
- Google Colab
- Matplotlib
- Breadth-First Search

## Testing

I tested the navigation algorithm using more than one obstacle layout.

The robot successfully found a route in the modified environment and reached the goal in 8 moves.

I also checked that:

- Every movement was to an adjacent cell.
- The route reached the intended goal.
- The robot did not move through obstacle cells.
- The algorithm continued to work after changing the obstacle layout.

## Limitations

This is a software simulation rather than a physical robot.

The current version does not simulate:

- Real sensors
- Motor movement
- Battery limitations
- Physical dimensions
- Wheel dynamics
- Sensor noise
- Unexpected obstacles

The environment is also known to the robot in advance.

## What I Learned

Through this project I learned how to represent an environment using coordinates, check whether movements are possible, implement BFS pathfinding, reconstruct a route, and visualize the result.

## Future Improvements

Possible future improvements include:

- Implementing A* pathfinding.
- Comparing BFS and A* performance.
- Generating random obstacle layouts.
- Animating the robot's movement.
- Adding simulated sensors.
- Introducing different movement costs.

## Project Status

Completed first version.

This project was developed as an independent student project to explore robotics and computer science.
