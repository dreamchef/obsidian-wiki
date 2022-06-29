---
id: 1ugju1nrlau13cd4akyd0lk
title: Exact Number of Properties
desc: ''
updated: 1656452270945
created: 1654530814468
---
#combinatorics

The number of objects having exactly $m$ properties if there are $r$ properties and $m \leq r$, is given by
$$e_m = s_m - {m+1\choose1} s_{m+1} + {m+2\choose 2}s_{m+2} - {m+3\choose 3}s_{m+3} \pm ... + (-1)^p {m+p\choose p}s_{m+p} \pm ... + (-1)^{r-m}{m+r-m\choose r-m} s_r$$

Notes:
- $s_t= \sum N(a_{i_1}a_{i_2}...a_{i_t})$
- taken that $s_0 = N$

