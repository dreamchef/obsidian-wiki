
#algorithms 

# Computation
## [[dynamic programming]]:
Complexity is $\theta (n^2)$.
```
for(int n=0; n<=Levels; n++)
{
	for(int k=0; k<=n; k++)
	{
		if((k==0) || (k==n))
			B[n][k];
		else
			B[n][k] = B[n-1][k-1] + B[n-1][k];
	}
}
```

