
#analysis

$e = \lim_{n \rightarrow \infty} (1 + \frac{1}{n})^n = \sum_{n=0}^\infty \frac{1}{n!}$

*Proof:* We begin by using the Monotone Convergence Theorem.  Expanding using the Binomial Theorem,

$$a_n = (1 + \frac{1}{n})^n = \sum_{k=0}^n {n\choose k} \frac{1}{n^k}$$

Now observe that 


$$\begin{align} 
	{n\choose k} \frac{1}{n^k} &= \frac{n!}{k! (n-k)!} \frac{1}{n^k} \\ \\
	&= \frac{n(n-1)...(n-k+1) (n-k)!}{k! (n-k)!} \frac{1}{n^k} \\ \\
	&= \frac{1}{k! } \frac{n(n-1)...(n-k+1)}{n^k} \\ \\
	&= \frac{1}{k! } \frac{n}{n} \frac{n-1}{n} \frac{n-2}{n} ... \frac{n-k+1}{n} \\ \\
	&= \frac{1}{k! } 1 (1-\frac{1}{n}) (1-\frac{2}{n}) ... (1-\frac{k+1}{n} \\ \\
	&< \frac{1}{k!} \tag{2}
\end{align}$$

Using inequality (2) on equation (1) gives the following
$$
\begin{align}
	a_n &= \sum_{k=0}^n {n \choose k} \frac{1}{n^l} \\ \\
	&\leq \sum_{k=0}^n \frac{1}{n^k} = s_n
\end{align}
$$
