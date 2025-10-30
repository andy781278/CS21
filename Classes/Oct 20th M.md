One of the [[Classes]]

#### [[Linearity of Expectation]]
Child shuffles 20 letters into 20 addressed envelopes, what chance correct letter goes in correct envelope, i=20

$X_i = \left\{ \begin{array}{rcl} 1 & \mbox{if} & envelope_i & is filled correctly\\ 0 & \mbox{otherwise}  \end{array}\right.$

$X=X_1+X_2+...+X_i$ by linearity of expectation

$E(X) = E(X_1)+E(X_2)+...+E(X_i) = \frac{1}{20}+\frac{1}{20}... = 1$
![[Screen Shot 2025-10-20 at 9.03.35 PM.png]]

![[Screen Shot 2025-10-20 at 9.05.07 PM.png]]

I suppose the process is as follows:

1. Define $X_i$ where X is the thing you are looking for, and $X_i$ is a way to divide up the X into small individual things with probabilities you can calculate
2. Make a rule stating X_i is 1(true) if it satisfies the requirements requested
3. find Probability of X_i at 1, or find the probability of a single instance being true
4. It probably is uniform, so we then add all the expected values of the individual X_i together

[[Oct 22nd W]]