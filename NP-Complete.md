---
id: 1k4xspf8je7zscdyqfhoxoo
title: NP-Complete
desc: ''
updated: 1656514097459
created: 1654530812065
---
#algorithms 

Class of problems for which exponential-time algorithms exist and polynomial time algorithms may or may not exist.

# Problems
- Traveling salesman
- Hamiltonian circuits
- Graph m-coloring
- 0-1 Knapsack
- Hamiltonian things
- K clique

# Proving a Problem is NP-Complete
1. Convert problem from optimization problem to "equivalent" decision problems (super easy)
2. Difficulty upper-bound: Show the problem is in NP [[nondeterministic polynomial]]
3. Difficulty lower-bound: Show it's in NP-Hard  (i.e. $HC \propto TSP$) by creating an algorithm that does the following:
	1. Reduce a known NP-Complete problem instance to an instance of the problem in question.
	2. Runs in polynomial time
