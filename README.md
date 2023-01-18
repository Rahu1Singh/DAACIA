# DAA CIA

QUESTION:

	find the shortest path from the starting node S to all other nodes
	Please submit the github repository link as part of CIA submission. Also, upload a note to the github, regarding the following:
		1. The shortest path from source node to all possible nodes with PRIMS, KRUSKALS, DIJKSTRA'S algorithms using C/C++/Python/Java. Give a justification for the choice of the programming language.
		2. Give a note of comparison regarding the performance of the algorithms. If you feel that any of the algorithms fail to find any of the required paths, give justification for the same.

NOTES:
	
	Language:
		Python - because I have never tried these algorithms on it.

	Prim's and Kruskal's Algorithms:
		1. Prim's and Kruskal's Algorithm cannot be used as they are used to find the minimum spanning tree, which is not the solution to the problem.
		2. Prim's Algorithm considers all vertices to be connected, which is true in case of the question but need not be for all directed graphs.
		3. Kruskal's Algorithm could assume cycles that are actually not present, for example D-A-C.	
	
	Dijkstra's Algorithm:
		Even though Dijkstra's algorithm works on this problem giving the correct solution, it wont work for all directed graphs with negatively weighted paths beacuse of its Greedy Approach.

SOLUTION:

	So to solve this problem, we use Bellman-Ford Algorithm, which can work even in case of directed graphs and negative weights.
	Bellman-Ford uses a bottom-up approach such that if the shortest path with i edges can be calculated, then the shortest path with i+1 edges can be calculated.
	
