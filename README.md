# Travelling Salesman Problem

This repo presents a quick comparison of the python implementation of three algorithms solving the travelling salesman problem:
- Brute force: Exhaustive Search Algorithm
- Greedy method: Nearest Neighbour Algorithm
- Greedy method: Repeated Nearest Neighbour Algorithm

Why? This jupyter notebook was developed for a short introductory project from the Maths and Physics Bachelor at La Sorbonne.

## The Algorithms

### Exhaustive Search Algorithm
This algorithm generates all possible paths between a given set of nodes/cities and returns the shortest one. While it guarantees to find the best path, its complexity is proportional to `(n-1)!` where `n` is the number of nodes/cities, making it highly impracticle for larger maps.

### Nearest Neighbour Algorithm
This algorithm arbitrarily chooses a starting point and goes from node to node chosing the nearest neighbour available. It does not guarantee to return the shortest path in the least but is significantly faster than the exhaustive method, making it more adequate for larger maps.

### Repeated Nearest Neighbour Algorithm
This algorithm repeats the Nearest Neighbour Algorithm for every starting point available. It is `n` times slower than the Nearest Neighbour Algorithm but the larger the map, the larger the probability it returns a shorter path while remaining vastly faster than the Exhaustive Search Algorithm.

## Results
The results folder contains all the maps generated and solutions found by each algorithm for the purpose of the project. The largest map tested contained "only" 13 nodes due to this map alone taking 80 minutes to be solved...

## What's next?
