---
id: 3b0egcgr0lnb4obtic46o20
title: Branch and Bound
desc: ''
updated: 1656443768387
created: 1654530812521
---
#algorithms #paradigm
# For Breadth-First Search
```
void breadth_first_branch_and_bound (state_space_tree T, number& best)
{
	queue_of_node Q;
	node u, v;
	
	initialize(Q);
	v = root of T;
	enqueue(Q, v);
	best = value(v);
	while (! empty(Q)){
		dequeue(Q, v);
		for (each child u of v){
			if (value(u) is better than best)
				best = value(u);
			if (bound(u) is better than best)
				enqueue(Q, u);
		}
	}
}

```
# For [[Best-First Search]]
```
void best_first_branch_and_bound (state_space_tree T, number& best)
{
	priority_queue_of_node PQ;
	node v, u;
	
	intialize(PQ);
	v = root of T;
	best = value(v);
	insert(PQ, v);
	
	while( !empty(PQ))
	{
		remove(PQ, v);
		if (bound(v) is better than best)
		{
			for (each child u of node v)
				if (value(u) is better than best)
					best = value(u);
				if (bound(u) is better than best)
					insert(PQ, u);
		}
			
	}
}
```
