# Graphs

A **graph** is a non-linear data structure that consists of **vertices** (or nodes) connected by **edges**, which can be visualized as line segments.

## Graph Terminology:

- **Vertex:** Also known as a "node," a vertex is a data entity that can have connections to other vertices.
- **Edge:** An edge signifies a linkage between two nodes.
- **Neighbor:** Neighbors are nodes connected by an edge.
- **Degree:** The degree of a vertex denotes the count of edges connected to it.

## Types of Graphs:

- **Undirected Graphs:** Edges in an undirected graph lack direction; connections are bidirectional.
- **Directed Graphs (Digraphs):** In a digraph, every edge has a direction.

## Graph Connectivity:

- **Complete Graphs:** All nodes are linked to each other.
- **Connected Graphs:** All nodes have at least one edge.
- **Disconnected Graphs:** Some nodes lack edges.

## Graph Cycles:

- **Acyclic Graphs:** Directed graphs without cycles.
- **Cyclic Graphs:** Graphs with cycles, which are paths that loop back to the same node.

## Graph Representation:

Graphs can be represented through:

- **Adjacency Matrix:** A 2D array where cells indicate connections.
- **Adjacency List:** A collection of lists/arrays noting adjacent nodes.

## Weighted Graphs:

Weighted graphs assign values (weights) to edges, indicating distances, costs, etc.

## Graph Traversals:

Two common traversal methods:

- **Breadth-First:** Visits nodes by levels, using a queue. Prevents cycles with a visited set.
- **Depth-First:** Uses a stack to visit nodes, focusing on subtrees.

## Real-world Applications:

Graphs are widely used in:

- **GPS and Mapping:** Finding routes and distances.
- **Social Networks:** Modeling relationships.
- **Recommendation Systems:** Suggesting products/services.
- **Airline Traffic:** Flight connections and routes.

In summary, graphs are a fundamental data structure with versatile applications in diverse fields due to their ability to model connections and relationships between entities.
