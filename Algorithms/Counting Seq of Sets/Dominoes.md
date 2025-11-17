#Algorithm 

How many 2x1 domino tilings are there in a 2xn space?
Let DT(n) be the number of domino tilings in a 2xn space

| DT(1) | DT(2) | DT(3) | DT(4) | DT(5) |
| ----- | ----- | ----- | ----- | ----- |
| 1     | 2     | 3     | 5     | 8     |
All domino tilings = start with 1 vert + start with 2 hor
start with vertical = DT(n-1)
start with horizontals = DT(n-2)
DT(n) = DT(n-1)+DT(n-2)
