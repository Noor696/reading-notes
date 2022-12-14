## Graphs

A **graph** is a non-linear data structure that can be looked at as a collection of **vertices** (or **nodes**) potentially connected by line segments named **edges**.

-> **_Vertex_** - also called a “node”, is a data object that can have zero or more adjacent vertices.

-> **_Edge_** - a connection between two nodes.

-> **_Neighbor_** - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.

-> **_Degree_** - The degree of a vertex is the number of edges connected to that vertex.

* **Undirected Graph** is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

* **Directed Graph** also called a **_Digraph_** is a graph where every edge is directed.

* **types of graphs depends on how connected the graphs are to other node/vertices:**

  - **Complete Graphs** : is when all nodes are connected to all other nodes.

  - **Connected graph** : is graph that has all of **_vertices/nodes_** have at least one edge.

  - **Disconnected graph** : is a graph where some vertices may not have edges.


* **Acyclic vs Cyclic:**

  - **Acyclic Graph** : is a directed graph without cycles , A cycle is when a node can be traversed through and potentially end up back at itself.

  - **Cyclic Graphs** : A Cyclic graph is a graph that has cycles, A cycle is defined as a path of a positive length that starts and ends at the same vertex.

* **represent graphs through:**

  - Adjacency Matrix :  is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix.

  - Adjacency List :  is a collection of linked lists or array that lists all of the other vertices that are connected.
