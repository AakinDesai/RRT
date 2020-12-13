# RRT

Rapidly-exploring random trees (RRT) creates both graph and finds a path. The path will not necessarily be optimal.

Points are randomly generated and connected to the closest available node. Each time a vertex is created, a check must be made that the vertex lies outside of an obstacle. Furthermore, chaining the vertex to its closest neighbor must also avoid obstacles. The algorithm ends when a node is generated within the goal region, or a limit is hit.

The method of determining a random position is a design decision. Method selected used here is random number generators. For basic applications, such approaches suffice.
