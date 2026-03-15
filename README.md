# Dijkstra's Shortest Path Algorithm

A program that finds the shortest path in a weighted undirected graph using Dijkstra's Algorithm, with graph visualization on Google Colab.

## Features

- Upload a `.txt` file to define the graph structure
- Compute the shortest path between any two nodes
- Visualize the graph with NetworkX, highlighting the shortest path in red
- Display a step-by-step distance calculation

## Input File Format

The `.txt` file should follow this format:

```
<number_of_edges>
<node1> <node2> <weight>
...
```

Example:

```
5
A B 4
A C 2
B D 3
C D 1
D E 7
```

- First line: total number of edges
- Following lines: source node, destination node, and weight (space-separated)
- Comments are supported using `#`
- The graph is undirected (edges work in both directions)

## How to Use

1. Open the program in Google Colab
2. Run all cells — a file upload dialog will appear
3. Upload your graph `.txt` file
4. The initial graph visualization is displayed
5. Enter a start node and an end node (A–Z)
6. The program outputs the shortest path, total distance with a step-by-step breakdown, and a graph visualization with the path highlighted

## Dependencies

- `heapq` — Priority queue for Dijkstra's algorithm
- `networkx` — Graph creation and manipulation
- `matplotlib` — Graph visualization

## Installation (outside Colab)

```bash
pip install networkx matplotlib
```

> **Note:** The `google.colab.files.upload()` function only works in Google Colab. To run locally, replace the file upload section with a direct file read.
