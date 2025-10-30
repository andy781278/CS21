one of the [[Classes]]

#### How to count $\sum_{k=0}^{n}\binom{n}{k}2^{k}$
$\binom{n}{k}$ means number of [[Fixed Density]] n length binary string with k ones.
$2^k$ means how many binary strings of length k

multiply together means that you need them both, in this case we can put them in an ordered pair, with $\binom{n}{k}$ on the left, and $2^k$ on the right, like $(\binom{n}{k},2^k)$

to combine them, think that k is the same, k is the number of ones for left, and length of string for right, so what if we match them up, for every one on the left, we add the string from the right, making some possibly a two. This makes sense, and the expression then counts all the strings of length n that has k non-zeros and has alphabet of 0, 1, and 2.

$\sum_{k=0}^{n}\binom{n}{k}2^{k}$ counts all ternary strings of length n and has n-k zeros

#### [[Conditional Probabilities]]

#### [[Bayes' Theorem]]

#### [[Law of Total Probability]]

[[Oct 15th W]]