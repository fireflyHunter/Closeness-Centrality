# Closeness-Centrality
￼DEVELOPER INSTRUCTION

1. Code analysing

The code of project include 3 parts:

(def shortest_path)
Count the shortest paths between a given vertex and all other vertexes in the graph.

(def calculate_sssp)
Count all the shortest paths by invoking (def shortest_path) in a for loop and store the results in a map as the return value.

(def loadData)
Load data from a csv file and store the data in a graph as return value.

2. Time Complexity

Calculating all the shortest paths in the graph is required in order to further
calculate the closeness centrality. 
For the N vertexes graph, there will be N*(N-1)/2 shortest path to be calculated, so the time complexity of this algorithm is (N²).

3. Develop environment

Java: >= 1.7. Download from “http://www.oracle.com/ technetwork/java/javase/ downloads/index.html”.
Scala: 2.10.x Should use this version or will cause problems.
Spark: >= 1.3. Download from “http://spark.apache.org/ downloads.html”. When upload java and scala into program, using the command “sbt/sbt assembly” in spark directory, create a jar package named “spark-assembly-***-***.jar” in dictionary “assembly/target/scala-2.10”.
IDE: Intellij idea. Download from “http://www.jetbrains.com/ idea/”.

￼
