---
id: veh3lr77qfqxj8g7frglke3
title: 0 1 Knapsack Problem
desc: ''
updated: 1656431952639
created: 1654530811533
---
#algorithms
# Problem
Given a **set of items** with weights and values, choose a subset that does not exceed a **given weight**, while maximizing value.

# Solutions
## [[backtracking]]:
### Intuition
How well could we **possibly** do by exploring past this node (in [[state space tree]])?  Proceed if we can do better than our current actual maxprofit.
### Pseudocode
```
void knapsack (index i, int profit, int weight)
{
	if (weight <= W && profit > maxprofit)
	{
		maxprofit = profit;
		numbest = i;
		bestset = include;
	}
	
	if (promising i)
	{
		include[i + 1] = "yes";
		knapsack(i + 1, profit + p[i + 1], weight + w[i + 1]);
		
		include[i + 1] = "no";
		knapsack(i + 1, profit , weight);
	}
}

bool promising (index i)
{
	index j, k;
	int totweight;
	float bound;
	
	if (weight >= W)
		return false;
	else
	{
		j = i+ 1;
		bound = profit;
		totweight = weight;
		while (j <= n && totweight + w[j] <= W)
		{
			totweight = totweight + w[j];
			bound = bound + p[j];
			j++
		}
		k = j;
		if (k<=n)
			bound = bound + (W - totweight) * p[k]/w[k];
		
		return bound > maxprofit;
	}
}
```
## [[branch-and-bound]]:
### Psuedocode
```
void knapsack3 (int n, const int p[], const int w[], int W, int& maxprofit)
{
	priority_queue_of_node PQ;
	node u, v;
	
	initialize(PQ)
	v.level = 0; v.profit = 0; v.weight = 0;
	maxprofit = 0;
	v.bound = bound(v);
	insert(PQ, v);
	
	while(!empty(PQ))
	{
		remove(PQ,v);
		if(v.bound > maxprofit)
		{
			u.level = v.level + 1;
			u.weight = v.weight + w[u.level];
			u.profit = v.profit + p[u.level;]
			
			if(u.weight <= W && u.profit > maxprofit)
				maxprofit = u.profit;
			u.bound = bound.u;
			if (u.bound > maxprofit)
				insert(PQ, u);
			
			u.weight = v.weight;
			u.profit = v.profit;
			u.bound = bound(u);
			
			if(u.bound > maxprofit)
				insert(PQ, u);
		}
	}
}
```
