Giraph_project
==============
Project includes Giraph 0.1 library. which is compiled with maven on Apache Giraph release version 0.1
compiled with hadoop version 1.2.0 to run on old hadoop version.


Included the shortest path algorithm code from giraph examples.

sample input data.
[0,0,[[1,1],[3,3]]]
[1,0,[[0,1],[2,2],[3,1]]]
[2,0,[[1,2],[4,4]]]
[3,0,[[0,3],[1,1],[4,4]]]
[4,0,[[3,4],[2,4]]]


To run this project you need to type following command.

giraph-0.1-jar-with-dependencies.jar library contains the Shoretest path code.

hadoop jar giraph-0.1-jar-with-dependencies.jar org.apache.giraph.examples.SimpleShortestPathsVertex /user/uxd120330/ginput/tiny_graph.txt /user/uxd120330/goutput/shoretestPathc2 0 3

hadoop fs -cat /user/uxd120330/goutput/shoretestPathc2/part*
