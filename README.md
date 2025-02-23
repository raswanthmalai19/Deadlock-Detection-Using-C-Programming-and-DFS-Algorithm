# Deadlock-Detection-Using-C-Programming-and-DFS-Algorithm

This repository contains a C program to detect deadlocks in a system using **Depth First Search (DFS)**. Deadlock detection is a crucial aspect of system resource management, ensuring that processes do not get stuck waiting indefinitely for resources.

## Features
- **Deadlock Detection**: Identifies cycles in the resource allocation graph to determine deadlocks.
- **Depth First Search (DFS)**: Utilizes DFS to detect cycles in a directed graph.
- **Dynamic Input**: Accepts user-defined processes and resources in a resource allocation graph.
- **Scalable**: Handles multiple processes and resources efficiently.

## Prerequisites
- A C compiler (e.g., GCC).
- Basic understanding of graph representation in data structures.

## How It Works
1. The program models the system as a **Resource Allocation Graph (RAG)**:
   - Processes and resources are represented as nodes.
   - Edges represent resource requests and allocations.
2. The graph is traversed using DFS to detect cycles:
   - If a cycle is found, a deadlock exists.
   - Otherwise, the system is deadlock-free.

compile :
gcc -o deadlock_detection deadlock_detection.c
./deadlock_detection

##Example:
 
Enter number of processes: 3
Enter number of resources: 2
Enter adjacency matrix:
0 1 0
0 0 1
1 0 0

so the output:
Deadlock detected! Processes involved: P1 -> P2 -> P3 -> P1
No deadlock detected.




## Applications:

Operating systems for detecting deadlocks in resource management.
Distributed systems to ensure smooth resource allocation.
Educational purposes for understanding graph traversal and system-level deadlock detection.

## Limitations:

The program assumes correct input format.
Limited to single-instance resources.
