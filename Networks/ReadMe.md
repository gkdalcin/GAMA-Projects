Although GAMA Platform presents a Graph class, such entity (as far as i researched) does not allow one to create
a graph using BOTH a shapefile containing the geometry of nodes with the numerical data on its load/potential AND a shapefile
containing the geometry of the connections between nodes with the numerical data on its impedance.
The creation of such kind of graph, with inputted numerical information on both its nodes and edges, is useful when
one wants to compute spatial metrics such as geometric accessibility and the Freeman-Krafta Centrality 
(https://www.researchgate.net/publication/23540856).
The algorithm here presented tries to solve such problem by importing the aforementioned shapefiles, using the Djikstra
algorithm (with a binary heap as priority queue) to find out the shortest path between all pair of nodes and lastly computing
the accessibility and Freeman-Krafta Centrality.
