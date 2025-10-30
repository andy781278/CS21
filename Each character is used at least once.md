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
