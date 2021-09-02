# BFS
Algorithm for searching a tree data structure for a node that satisfies a given property. It starts at the tree root and explores all nodes at the present depth prior to moving on to the nodes at the next depth level. Typically a queue is used to keep track of nodes encountered but not explored.

# Complexity Analysis
- Time Complexity: O(V+E) - Every vertex and edge will be explored in the worst case.
- Space Complexity: O(V) - Need space for all of the vertexes in the queue in the worst case.
