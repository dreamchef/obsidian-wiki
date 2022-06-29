---
id: lezurlf8fyjgzyf3smay9q9
title: Recurrence Relation
desc: ''
updated: 1656516270692
created: 1654530813648
---
#algorithms #combinatorics 

formula reducing later values of a sequence to earlier ones, with an initial condition
# Solutions
One recurrence relation may have many closed formulas, but initial conditions restrict these possible solutions.
## Substitution-Induction Method
1. Identify primary operation and find recurrence equation
2. Use substitution to identify possible closed form (Excel is great for this)
3. Use [[induction]] to prove closed form
## Characteristic Equation Method
1. Eliminate right-hand term if non-homogeneous
2. Write [[characteristic equation]]
3. Find roots and their [[multiplicity]]
4. Write general closed form
5. Apply initial conditions to solve for constants
## Using [[generating function]]
1. Multiply by $x^k$
2. Take infinite sum
