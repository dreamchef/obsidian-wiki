
#combinatorics #concept
# General form
the ordinary generating function is defined to be 
$$G(x) = \sum^\infty_{k=0}a_kx^k = a_0x^0 + a_1x^1 + a_2x^2 + ...$$
 
 something about polynomials? #q
 
 # Special cases
 ## Indistinguishable objects (5.2)
 Suppose we have $p$ types of indistinguishable objects with $n_i$ objects of type $i = 1, 2, 3, ... , p$. The number of ways we can choose $k$ objects when we can pick any number of objects of each type is given by the coefficient of $x^k$ in the generating function
 $$G(x) = (1 + x+ x^2 + ... + x^{n_1})(1 + x + x^2 + ... + x^{n_2})...(1 + x + x^2 + ... + x^{n_p})$$
Can be applied to [[occupancy problem]]
 
 # Method
 1. Set up polynomial factorization
 2. Expand
 3. Find coefficient of appropriate term
