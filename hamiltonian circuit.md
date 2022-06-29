
#combinatorics

# Finding a Circuit
## [[backtracking]]
```
if promising
{
	if (i == n-1) {
		done;
	}
	else {
		for(j = 2; j <= n; j++) {
			vindex[i + 1] = j;
			hamiltonian(i + 1);
		}
	}
}
```
# Existence
Suppose that G is a graph with $n \geq 3$ vertices and whenever vertices $x \neq y$ are not joined by an edge, the degree of x plus the degree of y is at least n.  Then G has a [[hamiltonian circuit]].
