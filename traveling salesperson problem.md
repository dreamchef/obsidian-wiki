
#algorithms #problem

# Algorithms
## [[branch-and-bound]]
### Intuition
#todo
### Steps
#### Calculate bound at node
adjacency matrix:
1. Cross out rows for from-vertices
2. Cross out columns to-vertices
3. Cross out entry for last edge
4. Sum minimum remaining edges in each row

### Psuedocode
``` bbts (...)
{
	priority_queu_of_node PQ;
	node v, u;
	
	initialize(PQ);
	v.level = 0;
	v.path = [1];
	v.bound = bound(v);
	minlength = inf;
	insert(PQ, v);
	while( ! empty(PQ))
	{
		remove(PQ, v); // remove something and assign it to v?
	}
}
