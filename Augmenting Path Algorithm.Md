
#combinatorics
1. Start with any [[matching]] $M$.
2. Select an unsaturated vertex $x$  from which you have not previously done a search. If there is no such vertex, you are done: the graph has no [[augmenting path]] and $M$ is maximum.
3. If there is such a vertex $x$, beginning there start a [[breadth-first search]] that builds an alternating tree. If you find no augmenting path, return to the previous step.
4. If you find an augmenting path $C$, perform [[augmentation]] to obtain a larger matching $M$.
5. Rename this new matching as $M$ and return to the first step.