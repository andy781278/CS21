one of the [[Classes]]
More knights and castles
11 knights in 5 castles
000100011000001
$\binom{15}{4}$
each knight takes 1 castle minimum
$\binom{10}{4}$
this is gotten from removing the 1 knight per castle first, then getting the config with the rest of the knights

what about this, but knights are unique?
$$\sum_{k=0}^{5}\binom{5}{k}(5-k)^{11}(-1)^k$$
The number of ways to put n knights into k castles is $\binom{n+k-1}{k-1}$
The number of ways to do this with 1 knights in each castle at least is $\binom{n-1}{k-1}$

#### [[Integer Equations]]
consider $a+b+c+d=10$ where a,b,c,d are non-negative integers, how many sol for eq?
consider each var a castle, and the constant the num of knights
therefore $\binom{10+4-1}{4-1}$
Differnt senario:
for general equation, $a_1+a_2+...+a_k = n$, where n and $a_i$ have to be **positive** ints
Now we have to make sure each var has at least 1
for each $1\leq a_i \leq n$, let $x_i = a_i -1$, that converts the og eq to $x_1+x_2+...=n-k$  where $n-k$ and $x_i$'s are non-negative
There are $C((n-k)+k-1,k-1) = C(n-1,k-1)$ solutions

Example:
$a_1+a_2+a_3+a_4=18$
- $\binom{21}{3}$ no restrictions
- $\binom{17}{3}$ at least 1 per var
- $\binom{15}{3}$ $a_1$ is bigger than 5, everything else same
- $\binom{21}{3}-\binom{15}{3}$ $a_1$ is less or eq to 5, everything else same, complement to the one before

#### [[The 12-fold way]]

Discussion
#### [[Combinatorial proofs]]
[[Bijection Proof]]
1. find a set counted by the LHS
2. find a set countd by the RHS
3. build a bijection between these two sets
Example
$\binom{n}{k} = \binom{n}{n-k}$
4. the set of all binary strings with length n and k 1s
5. the set of all binary strings with length n and n=k 1s
6. consider that the map that changes all 1s into 0s and all 0s into 1s, it is a bijection between two sets above

[[Same-Set Proof]]
1. Find a set <- define this first clearly (Let S be the set...)
2. explain why the LHS counts this set <- do 2 and 3 separately, no moving terms in between
3. explain why the RHS counts this set
Example
$\sum_{k=0}^{n} \binom{n}{k} = 2^n$
4. Let S be a set of all binary strings length n
5. $2^n$ counts the number of binary strings length n
6. We compute the Summation, creating a partition of many subsets added together. For example, all n length strings with k=0 ones, k=1 ones,..., k=n ones. This accounts for all n length strings
Problem
$\sum_{k=0}^{n} k \binom{n}{k} = n2^{n=-1}$
7. Let n be number of students, and set S be the set of all study groups formed by these n students, 1 of them has to be a leader
8. LHS: size of study group is k, so k ranges from 0 to n, next, pick k people from all n students (n choose k), finally, pick 1 leader from this study group (k)
9. RHS: pick leader from n students (n), then, pick a subset of remaining students, they are non-leader group membets ($2^{n-1}$)

[[Oct 10th F]]