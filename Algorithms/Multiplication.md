#Algorithm #DivideAndConquer
Note: O(n) for addition

Given a and b, both n digits, multiply them, what is the runtime?

you multiply each of the digits in b by whole of a, which is $n^2$ operations
then you add them, which is n-1 operations
in total, $O(n^2)$

Too slow, lets do divide and conquer
![[Screen Shot 2025-11-17 at 1.09.35 PM.png]]

Function Multiply(2 n digit integers of x and y): outputs xy
	if n=1: return x*y
	split x into $x_l, x_r$, and split y into $y_l,y_r$
	