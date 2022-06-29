---
id: rso2lntt0kx10w9qbknbspp
title: Register Allocation Problem
desc: ''
updated: 1656516332678
created: 1654530813661
---
#combinatorics 

Map many variables to few registers.

# Solution
This is reducible to [[graph m-coloring problem]] where
- vertices represent vaariables
- colors represent reigsters
- interference edges connect vertices which are alive at the same time
