#Sorting 

### WHAT
Given a list $[a_1,a_2,...,a_n]$
- for each element in the list (i from 1 to n):
	- Find the smallest element ($x_i$) in list
		- Go through the list, compare an arbitrary smallest so far to each element
	- swap $x_i$ with the smallest element
### WHEN
How many swaps for
- Best case: 0
- Worst case: n-1 (cyclically shifted by 1)
How many comparisons for
- BC/WC (they're the same amt): $1+2+3+4+...+(n-1) = \frac{n(n-1)}{2}$