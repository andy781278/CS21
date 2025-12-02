 #Graph
Graphs are mathematical objects/virtual data structures comprised of vertices and edges.

Graphs can be Directed or Undirected
Undirected - Degree Sum = 2 * edges
Directed - Indegree sum = Outdegree sum = edges

Walk: A route that alternates vertexes and edges
Trail: A walk that doesn't repeat edges
Path: A walk that doesn't repeat edges and vertices, Simple Path
Trivial Path: every vertex has a trivial path to itself with length 0
Closed Walk: A walk that starts and ends on the same vertex
Circuit: A trail that starts and ends on the same vertex, length > 0, closed trail
Cycle: Simple Path that starts and ends on the same vertex, length > 0, Closed path
Loop: An edge that points a vertex to itself
Complete Graph: A graph that connects every vertex to every edge, Undirected, $K_n$
Bipartite Graph: A graph with two sets of vertices $V_1, V_2$, and no vertices in the same set connects to each other
Tree (Undirected): an undirected, connected graph with no cycles
Tree (Directed): Rooted Tree, A directed graph with the property that each vertex has exactly 1 edge pointing to it, except for the root, which has zero.
Connected (Undirected): every point can go to every other point
Weakly Connected (Directed): if made into undirected, every pt can go to every other point
Strongly Connected (Directed): every pt can go to every other pt

![[Encoding Graph]]