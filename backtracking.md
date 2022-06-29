
#algorithms

a set of algorithms used to find, given a set of objects, a sequence of chosen objects that satisfies some criterion
# Pseudocode
```
void checknode (node v)
{
	node u;
	
	if (promising(v))
		if (there is solution at v)
			write solution; (done)
		else
			for (each child u of v)
				checknode(u);
}
```
In cases of optimization, perform algorithm on node, then check if it is promising to decide whether to perform algorithm on its children.
```
void checknode (node v) {
	
	node u;
	if (value(v) is better than best)
		best = value(v);
	if (promising(v))
		for (each cild u of v)
			checknode(u)
}
```