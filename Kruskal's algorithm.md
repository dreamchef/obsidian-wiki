---
id: bvlesp0t6g22naqhvbhu73y
title: Kruskal's algorithm
desc: ''
updated: 1656468814375
created: 1654530811954
---
#algorithms #combinatorics 

given a connected graph, finds a  minimum [[spanning tree]]

Complexity is $O(e \log e)$.
# Psuedocode
*Inputs:* $n \geq 2$ number of vertices,  $m$ number of edges and set $E$ of edges with weights

*Output:* F, set of edges in MST
```
void kruskal (int n, int m, edge E[], edge& F[])
{
	index i, j;
	set_pointer p, q;
	edge e;
	Sort m edges in E by weight, nondecreasing;
	F = null;
	initial(n); // Initialize n disjoint subsets.
	while (number of edges in F < n - 1)
	{
		e = edge with least weight not yet considered;
		i, j = indices of vertices connected by e;
		p = find(i);
		q = find(j);
		if ( ! equal(p,q)) {
			merge(p, q);
			add e to F;
		}
	}
}
```

## Steps
*Input:* a network G on n > 1 vertices

*Output:* a set of edges defining a minimum spanning tree of G or the message that G is disconnected

1. Arrange edges in nondecreasing queue
2. Initialize T (set of edges of MST)
3. If every edge of G has been examined, stop (disconnected).  Else, examine the first unexamined edge in the queue. Add it to T iff it does not form a circuit with some edges already in T, and go to step 3.  Otherwise, go to step 2.
4. If T has n - 1 edges, stop and output T.  Otherwise, go step 2.
