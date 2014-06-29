Graph-Visualization
===================

This is a fork of [David Piegza's Graph Visualization.](https://github.com/davidpiegza/Graph-Visualization/blob/master/Graph.js) 
The major (unmerged, as of yet) difference is that I modified SimpleGraph's positioning routines to not always start from a random position. 
This is useful when synchronizing visualizations between different clients (as we are doing.) Elements can be started at a random position, 
OR they can be started from a given position. The example for this was really tightly integrated into my other code base. If you need an 
example of this, shoot me a message or give me a call. 

A merged change I created was that disjoint subgraphs now no longer fly off to infinity. This has been accomplished by setting forces at
each timestep, as opposed to integrating forces (adding to the force each time step.) Repulsive forces are also inversely proportional to 
the square of the distances between nodes, as opposed to being inversely proportional to the distance between nodes.

So, to test this, check out disjoint_example.html. This sets a global variable var DISJOINT_EXAMPLE = true; to randomly not-add edges.

### Run the example ###

1. Clone or download the project
2. Open the disjoint_example.html in a WebGL-compatible browser

Look at [David Piegza's Graph Visualization.](https://github.com/davidpiegza/Graph-Visualization/blob/master/Graph.js) for more information. 
Please contact me if you're interested in any contract code modification! That's what I do as my full time job. Brian Stinar - 505-750-1169.
