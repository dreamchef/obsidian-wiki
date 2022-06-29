---
id: rjg5ig8u2iizh20y000n2n6
title: Hungarian algorithm
desc: ''
updated: 1656453109482
created: 1654530811927
---
#combinatorics 

given a graph, finds the minimum weight [[matching]]
# Pseudocode
*Input:* n-by-n integer matrix C

*Output:* A minimum-weight matching
```
// Intialization
// rows
for(i = 1: i <= n; i++) {
	p = smallest element in C[i];
	for(j = 1; j <= n; j++) {
		row[i][j] -= p;
	}
}
// cols
for(i = 1: i <= n; i++) {
	p = smallest element in ith col of C; // how to program?
	for(j = 1; j <= n; j++) {
		row[j][i] -= p;
	}
}
// Find lines
land findLines;
find minimum cardinalit set of lines covering the zeroes of cij;
k = size of set;
if(k < n) {
	find set of n independent 0s;
	This corresponds to the set of edges in a min-weight matching;
}
else {
	p = smallest uncovered element in C;
	subtract p from every uncovered element;
	add p to each double-covered element;
	jump findLines;
}
```
