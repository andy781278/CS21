#Sorting #Algorithm

### HOW
Divide and Conquer:
Divide the list into 2 sub-lists
Recursively sort each sublist
Conquer by merging the two sorted lists into a single list

RMerge(list 1, list 2): (size k, size l)
if nothing in list 1: return list 2
if nothing in list 2: return list 1
if e1 from list 1 < e2 from list 2: return e1 * RMerge(list 1 sans e1, list 2)
else: return e2 * RMerge(list 1, list 2 sans e2)

### WHAT

### WHY
How would you prove this algorithm is correct?
Regular Induction:
Base Case k+l = 0, then the alg returns nothing which is trivially sorted
Inductive Hypothesis: k+l = n for any n $\in \mathbb{R}^+$, Assume RMerge works for any two lists with the combined size of n-1. Consider two lists $[a_1,a_2,...,a_k]$ and $[b_1,b_2,...,b_l]$ such that k+l=n
Inductive Step: 
Case k=0 (list 1 empty): then alg returns list 2, which is sorted by ind hyp
Case l=0, same thing
Case k>0, l>0, $a_1<b_1$: 