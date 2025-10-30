one of the [[Classes]]
Proving the [[Sum Identity]]

Last time we talked about Inclusion-Exclusion property with the + and - sets that overlaps

#### **[[Each character is used at least once]]:**
How many n length strings over alphabet size X? $X^n$, power rule
How many n length strings over alphabet size X such that every character is used at least once?
length 3: 3!
length 4: the previous 3! but for each you can fit 3 more possibilities, so $3*3!$
length 5: this gets complicated...

Easy way to do this for length n?
Each character used at least once = a is used at least once AND b used at least once AND ...
something like $|a\cap b\cap c| = |All| - |\overline a \cup \overline b \cup \overline c| = |All| - [\overline |a| + \overline |b| + \overline |c| - |\overline a \cap \overline b| - |\overline a \cap \overline c| - |\overline b \cap \overline c| + |\overline a \cap \overline b \cap \overline c|]$
$\overline a$ is set of all strings without a
$\overline b$ is same and also for $\overline c$

Example, for length 12 3 characters:
$3^{12} - [2^{12}+2^{12}+2^{12} - 1^{12}-1^{12}-1^{12}+0^{12}]$
$\binom{3}{0} 3^{12} - \binom{3}{1} 2^{12} + \binom{3}{2} 1^{12} - \binom{3}{3} 0^{12}$
$=\sum_{k=0}^{3} \binom{3}{k}(3-k)^{12}(-1)^k$

General Formula:
$$\sum_{k=0}^{x}\binom{x}{k}(x-k)^n(-1)^k$$

#### [[Stars and Bars]]
Identical vs Distinct objects:
5 different knights into 3 castles, all of them has to go to a castle, more than 1 knight can be in 1 castle
$3^5$ arrangements, each knight has 3 choices, 5 knights in total.
Now, they are identical robot indistinguishable knights, what changes?
now the way to do it is to pretend they are on a line, fences separate castles that act as 1, and knights are 0, now we have a binary string with [[Fixed Density]]. 0010100 for example, so we're simply picking what positions for the 1 to go, so $\binom{7}{2}$. This only works if the castles are distinguishable.

If i have n knights and k castles, then I need:
n stars
k-1 castles
or n zeros and k-1 ones
$$\binom{n+k-1}{k-1}$$

Quiz stuff:
q4:
subsets of set {1,2,...,11} contains at least 1 odd and at least 1 even
we can rearrange eq to get total - no odd or no even = at least 1 odd and at least 1 even (demorgans law)
at least 1 odd is total - no odds. total subsets should be $2^{11}$ or 2048 subsets. No odds should be just evens, or 2,4,6,8,10, 5 numbers. subset with just evens... is equivalent to subset of set {2,4,6,8,10}, which should be $2^5$.
The evens is similar, but $2^6$ because {1,3,5,7,9,11} is 6 elements.
So this should be $2^{11}-2^5-2^6 = 2048-32-64=1953$

[[Oct 8th W]]