---
id: eowcbubyz1mmidv89clp6fl
title: task decomposition (MIMD)
desc: ''
updated: 1654530813942
created: 1654530813942
---
#algorithms #paradigm 
**Complexity:** [[NP-Complete]]
# Task graph
#q what was that about edge weights?
One start node and one edge node.  Each edge is a subtask.
## Critical path
takes the longest or something
## Sequential time
the sum of all edges
## Speedup
$$\frac{\text{Sequential Time}}{\text{Parallel Time}}$$
## Span
Greatest number of processors running simultaneously.
## Partitioning
Draws lines.  Each space contains the tasks the processor will do.
