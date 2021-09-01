# Topological Sort
Valid only for Directed Acyclic Graphs (DAG)

A topological sort is a graph traversal in which node v is visited only after all its dependencies are visited.

One implementation is to do a modified DFS, we recursively call DFS on each adjacent vertex of a given vertex, before pushing it to a stack. At the end, the stack is the reverse order return of the topological sort. 

### Complexity Analysis
Generally the complexity is as follows: 

- Time Complexity: O(V+E) - The algorithm calls all vertexes, and each edge will be traversed in the worst case. 
- Space Complexity: O(V) - Space needed to store the stack.