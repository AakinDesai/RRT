# RRT

Rapidly-exploring random trees (RRT) creates both graph and finds a path. The path will not be always optimal.

Points are randomly generated and then from the closest available node a specific amount of distance is travelled to create new vertex. Each time a vertex is created, a check must be made that vertex lies outside of an obstacle. Furthermore, chaining the vertex to its closest neighbor must also avoid obstacles. The algorithm ends when a node is generated within the goal region, or a limit is hit.

The method of determining a random position is a design decision. The method used here is random number generators. For basic applications, such approaches suffice.
