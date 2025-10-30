one of the [[Classes]]
[[r-Combinations]]
Set S with n elements, get subset of k different elements of S, order doesn't matter

n choose k, C(n,k), nCk

you can turn C to P by multiplying by k!

C(n,k) counts the number of
- k element subsets of a set of cardinality n {1,2,...,n}
- length n binary strings with exactly k ones

these two are a bijection, bc 1 to 1 and unto

{1,2} <-> 1100
{3,4} <-> 0011

if n=8 and k=3, how many [[Fixed Density]] binary strings are there for 8 length string with 3 ones
- number of ways you can choose 3 out of 8 positions
- number of ways to make anagrams with 3 ones and 5 zeros
same thing as before, that's why theres bijection

Problem
6 by 3 grid, start bottom left, can only go up or right, to get to top right
9 choose 3 or 9 choose 6

1. $10^2*8$
2. $10*9*8$
3. $10C2 * 8$

4. $5^4$
5. $5^3 * 2$
6. $4^3 * 4$
7. contains at least 2 even digit = total - contains 1 - contains 0
	1. total = $5^4$
	2. contains 1 = 2 _ _ _ , 4 _ _ _ , _ 2 _ _ ,... $(2*(4^3))^4$
	3. contains 0 = $3^4$
	4. ans = $5^4 - 2*3^3*4 - 3^4$
8. total - X345 - 345X = $5^4 - 10
9. start where you want and go from there
	1. 5 c 3, choose the numbers you want from the list
	2. 3 c 1, choose which one to have 2 copies of
	3. 4 c 2, 4 positions, choose 2 to put the repeating numbers
	4. 2 c 1, 2 positions left, pick 1 for one of the left over numbers
	5. 1 c 1, only 1 position left and 1 number left

[[Induction]]

[[Oct 3rd F]]