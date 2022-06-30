
#algorithms #combinatorics  

Find a way to color an indirected graph using ***at most*** m different colors, so that no two adjacent vertices are the same color.

This problem has duality with the [[N-Queens Problem]].

# Solutions
## [[backtracking]]
### Intuition
[[state space tree]] where...
- each level represents a vertex in the actual graph
- the tree's distinct vertices represent colors
- the tree is pruned based on the existence of edges in the graph

### Algorithm
```
void m_coloring (index i)
{
	int color;
	
	if (promising(i)) {
		if (i==n)
			cout << vcolor[1] through vcolor[n]
		else
			for (color = 1; color <= m; color++) {
				vcolor[i+1] = color;
				m_coloring(i+1);
			}
	}
}

bool promising (index i)
{
	index j = 1;
	bool switch = true;
	
	while(j < i && switch) {
		if(W[i][j] && vcolor[i] == vcolor[j])
			switch = false;
		j++;
	}
	return switch;
}
```
