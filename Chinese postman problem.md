
#combinatorics

Given a graph G, find the optimal multigraph H.
# Solutions
- Add copies of vertices to create a graph with a eulerian circuit:
	1. Create a graph G' that includes the vertices of odd degree from G, with weighted edges between each pair of odd vertices.  The weights are given by the weights of the shortest paths between the odd vertices in G		
	2. Find a perfect matching of G'.
	3. Add copies of edges to G corresponding to the matching found in step 2.
	4. The result is the optimal multigraph H.
- [[Hungarian algorithm]]
