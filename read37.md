# Graphs

A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

Here is some common terminology used when working with Graphs:

* Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.

* Edge - An edge is a connection between two nodes.

* Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.

* Degree - The degree of a vertex is the number of edges connected to that vertex.

**Types of graphs:**

**Undirected Graph**

![un](https://www.researchgate.net/profile/Hakan-Terelius/publication/265428782/figure/fig3/AS:669498856194058@1536632374537/An-undirected-graph-with-7-nodes-and-7-edges.png)

**Directed Graph**

![di](https://www.researchgate.net/profile/John-Lee-156/publication/220863116/figure/fig1/AS:669516962988037@1536636691241/An-example-of-a-directed-graph-with-9-nodes.png)

**Acyclic vs Cyclic**

Acyclic Graph is a directed graph without cycles.

cycle is when a node can be traversed through and potentially end up back at itself.A directed acyclic graph is also called a DAG.

Cyclic Graphs is a graph that has cycles. A cycle is defined as a path of a positive length that starts and ends at the same vertex.

**Weighted Graphs**

is a graph with numbers assigned to its edges. These numbers are called weights.

**Breadth First**

In a breadth first traversal, you are starting at a specific node. This node should be specified when calling the BreadthFirst() method. The breadth-first traversal of a graph is like that of the tree, the difference is the graphs can have cycles. When a graph has cycles and we are trying to traverse, this leaves possibility to be in an infinite ,which is bad. To prevent this, we need to had some sort of flag that specifies if we have already visited that vertices. Upon each visit, we just set the “visited” flag from false to true.

**Depth First**

In a depth first traversal, we approach it a bit different than the way we do when working with a depth first traversal of a tree. Similar to how the breadth-first uses a queue, we will use a Stack for our depth-first traversal.