One of the [[Classes]]

#### Partition the Sample Space
[[Law of Total Probability]] states:
Let $\{B_1,B_2,...,B_k\}$ be the partition of sample space S such that any two $B_k$ are mutually exclusive and all B add to S

Then for any event A:
$$P(A) = \sum_{i=1}^{k}P(A|B_i)P(B_i)$$
##### Independent Events
Events are independent iff $P(E\cap F) =P(E)P(F)$
This means change in one does not change the other
Independent is not disjoint, so don't assume and prove it

##### Rejection Sampling
If you want to pick a certain T $\subseteq$ S, pick a random element x of S, see if x $\in$ T, if not then repeat

[[Oct 17th F]]