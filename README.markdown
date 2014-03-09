Graph-Visualization
===================

This is a fork of [David Piegza's Graph Visualization.](https://github.com/davidpiegza/Graph-Visualization/blob/master/Graph.js) 
The major difference is that disjoint subgraphs now no longer fly off to infinity. This has been accomplished by setting forces at
each timestep, as opposed to integrating forces (adding to the force each time step.) Repulsive forces are also inversely proportional to 
the square of the distances between nodes, as opposed to being inversely proportional to the distance between nodes.

So, to test this, check out disjoint_example.html. This sets a global variable var DISJOINT_EXAMPLE = true; to randomly not-add edges.

This project is about 3D graph visualization with WebGL. The aim of this project is to evaluate the possibilities of graph drawing in WebGL.

This project uses Three.js for drawing and currently supports a force directed layout.


### Run the example ###

1. Clone or download the project
2. Open the disjoint_example.html in a WebGL-compatible browser

Look at [David Piegza's Graph Visualization.](https://github.com/davidpiegza/Graph-Visualization/blob/master/Graph.js) for more information. 
Please contact me if you're interested in any contract code modification! That's what I do as my full time job. Brian Stinar - 505-750-1169.