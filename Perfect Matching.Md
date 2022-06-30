
#combinatorics  

a matching in which every vertex is saturated

# Solution
*Input*: A graph G with 2n verticse and each vertex having $\geq$ n.

*Output*: [[Perfect matching]] of G

```
M = null
while(there is an unsaturated pair of vertices in G, joined by an edge in G)
	Place pair into M.
until(M has n edges)
{
	Find a pair {a,b} of unsaturated vertices in G (!joined by edge in G)
	Find edge {u,v} in M s.t. {a,u} and {b,v} are edges of G
	Remove {u,v} from M and places edges {a,u} and {b,v} in M
}
output M
	
```
