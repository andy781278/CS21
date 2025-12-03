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

Eulerian Trail is a trail where each edge occurs exactly once (Easy to find)
- Eulerian Circuit is a Eulerian Trail that starts and ends on the same vertex
- degree of intermediate vertexes must be even
- has either 0 or 2 odd-degree vertices
- connected
- Finding Eulerian Trail
	1. Find the 2 odd-degree vertices
	2. Start from one of them, and loop:
		1. go down an edge that's not a bridge (when removed, graph becomes disconnected)
		2. After going, remove the edge that was just went, and update the degrees accordingly, there should now still be either 0 or 2 odd degree edges
		3. Choose a new edge from the new vertex, be sure to also not choose a bridge
		4. Visit every node on that side of the bridge before crossing the bridge\
		5. Do the same on the other side

Hamiltonian Path is a path where each vertex occurs exactly once (Hard to find)

Directed Acyclic Graph (DAG)
- A directed graph with no cycles
- When there is cycles, there is no good ordering for the vertices
- Topological Ordering or Linearization of a graph is a sorted list of all its vertices such that for each edge $(v,w)$ in the graph, v comes before w in the list
- vertices with no incoming edges: Sources
- vertices with no outgoing edges: Sinks
- Make a Topological Order:
	1. While there are still sources:
		1. run through the sources, output them, then remove them and their outgoing edges, update this to make new sources

![[Encoding Graph]]