#class
Correct answer from [[Sep 26th F]]'s question: $(62^8-36^8)$
Explaination:
- imagine circle that represents the total number of possible permutations of 8-lettered passwords, that circle contains $62^8$ passwords
- The circle then can be composed of passwords with at least 1 upper case letter, and passwords with no upper case letters
- rearrange equation, and you can retrieve # passwords with >=1 upper case letter by subtracting # passwords with no cap from total

More examples
1. How many 4 digit strings number 0-9 have at least 1 zero?
	a. $4*9^3$ exactly 1 zero
	b. $10^4-9^4$ correct
	c. $4*9^3 + 6*9^2 + 4*9^1 + 1*9^0$ add together exact 1, exactly 2 ... exactly 4 zeros
	d. $10^3+9*10^2+9^2*10+9^3$ counts based on 0 position:
		$10^3$  means the first one is 0, so the rest is any
		$9*10^2$ means that the 0 is on the second one, and the first one can't be 0, 
		$9^2*10$ means that 0 is the third one, and first 2 cant be 0
		the last one means all 3 before can't be 0
		so the zero goes from left to right, and everything to its right counts 0, and everything to its left don't
		If we counted 0 on the left, then there will be repeats, for example, A0XX and 0XXX, if A can be 0, then there will be 2 counts of 00XX, which can't be.
		However, if we can't have 0 on the left, then theres no way to repeat
		So a way to think about it would be to have the left include 0, then get rid of it in the end, turning it into 9 from 10.
	e. $4*10^3$ exactly 1 "red" zero, with other digits being blue
2. How many ways can you distribute 10 different candies to 4 children?
	a. $4^10$ correct
	b. $10^4$
	c. $10*9*8*7$
	d. $10*4$
	e. $10*(4*3*2*1)$

Try to imagine slots with underline _ _ _ _

[[r-Permutations]]
number of ways to arrange r objects out of n positions/spots/slots
P(n,r) = nPr = n(n-1)(n-2)...(n-r+1) = $n! / (n-r)!$ 

[[Permutations]]
rearrangements/ordering so each obj appears exactly once

[[Multiset]] a collection that allows repeats
example: {1,1,2,3} is a [[Multiset]] because 1 repeats

[[Anagram]] for repeating letters


[[Oct 1st W]]