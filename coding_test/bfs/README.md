Breadth-first search (BFS) is an algorithm for traversing or searching tree or graph data structures. It starts at the tree root (or some arbitrary node of a graph, sometimes referred to as a ‘search key’) and explores the neighbor nodes first, before moving to the next level neighbors.

Here is an example of a Python implementation of BFS using a queue data structure:

```python
from collections import deque

def BFS(graph, start):
    visited = set()
    queue = deque([start])
    visited.add(start)

    while queue:
        vertex = queue.popleft()
        print(vertex)
        for neighbor in graph[vertex]:
            if neighbor not in visited:
                visited.add(neighbor)
                queue.append(neighbor)

graph = {'A': ['B', 'C'],
         'B': ['A', 'D', 'E'],
         'C': ['A', 'F'],
         'D': ['B'],
         'E': ['B', 'F'],
         'F': ['C', 'E']}

BFS(graph, 'A') # A B C D E F
```

In this example, the BFS function takes two arguments: the graph which is represented as an adjacency list and the start node. 
The function initializes a set visited to keep track of the visited nodes, and a queue queue to hold the nodes to be visited. It starts by adding the start node to the visited set and the queue.

The function then enters a while loop, where it takes the first node from the queue, prints it and visits all its unvisited neighbours. 
The neighbours are added to the queue and the visited set. The loop continues until the queue is empty.

One advantage of breadth-first search (BFS) is that it guarantees that the shortest path will be found first. 
Because BFS explores the neighbor nodes first before moving on to the next level of neighbors, 
it will always discover the shortest path from the starting node to the goal node (if one exists) before discovering any longer paths. 
This makes BFS useful for finding the shortest path in problems such as the shortest path in a graph or to find the minimum number of steps needed to reach a goal state in a tree or graph.


