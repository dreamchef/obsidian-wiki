---
id: 3jzueoyfjf4q2zaxort4z19
title: Depth First Search
desc: ''
updated: 1656450972123
created: 1654530812824
---
#combinatorics #algorithms
# For Connectedness
Complexity is $n^2 + n$.
1. ***Start*** from a random vertex.
2. Go down a random path until reaching a vertex of whom all. neighbors are visited.
3. Backtrack to a vertex with an unvisited neighbor.
4. ***Repeat*** 2-3 until
	a. Back at start without visiting all vertices $\rightarrow$ unconnected
	b. Visited all vertices $\rightarrow$ connected
