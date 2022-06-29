---
id: rlmdp4gudjavt7vny9cvq98
title: Dijkstra's algorithm
desc: ''
updated: 1656451241678
created: 1654530811731
---
#algorithms

Given a weighted graph and two vertices, find the the minimum-weight route between them.

Complexity is $O(n^3)$.

# Steps
Given a directed network $D$ and vertices $x$ and $y$ from $D$, the algorithm outputs the shortest path from $x$ to $y$ or the message that there is no path from $x$ to $y$.
1. Place vertex $x$ in the class $W$, let $B = null$, and let $d(x,x) = 0$.
2. 
	1. For each vertex $u$ in $W$ and each vertex $v$ not in $W$, let $\alpha(u,v)=d(x,u) + w(u,v)$.  Find $u$ in $W$ and $v$ not in $W$ such that $\alpha(u,v)$ is minimized.  Choose arbitrarily in case of ties.
	2. If the minimum step 2.1 is infinity, stop and give the message that there is no path from $x$ to $y$.
	3. Else, place $v$ in $W$ ($v$ being the next vertex chosen), place arc $(u,v)$ in $B$, and set $d(x,v)$ = $\alpha(u,v)$
3. If $y$ is not yet in $W$, return to step 2.  Otherwise, stop.  A shortest path from $x$ to $y$ can be found by using the *unique path of arcs B* that goes from $x$ to $y$.

