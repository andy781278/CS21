#Algorithm #DivideAndConquer 
bit strings can only have 0s or 1s.
n-bit strings are bit strings of size n

Let BS(n) be the number of n bit strings
Count the set of n-bit strings by separating them
all n-bit strings = start with 0 + start with 1

BS(n) = 2BS(n-1)
BS(0) = 1

Unraveling:
1 BS(n) = 2BS(n-1)
2 BS(n) = 2(2BS(n-2)) = 4BS(n-2)
3 BS(n) = 2(4BS(n-3)) = 8BS(n-3)
k BS(n) = $2^kBS(n-k)$
n BS(n) = $2^nBS(n-n) = 2^n$ 
