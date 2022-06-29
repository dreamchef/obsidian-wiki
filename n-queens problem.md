---
id: 9zza7imwbc6ibwoqxkjwrnx
title: N Queens Problem
desc: ''
updated: 1656513033817
created: 1654530813402
---
#algorithms

Place n queens on an n by n chess board so that no two queens threaten eachother.
# Solution
Complexity of an exhaustive approach is $O(n^n)$.
## [[backtracking]]:
Complexity is $O(nlog_4n)$.
### Psuedocode
```
void queens (index i)
{
	index j;
	
	if (promising(i))
		if ( i==n )
			cout << col[1] through col [n];
		else
			for (j = 11; j <= n; j++){
			#todo 
			}
}
```
When implementing this, compare column and row differences to determine diagonal conflicts.
