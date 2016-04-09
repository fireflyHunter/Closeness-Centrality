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
For the N vertexes graph, there will be N*(N-1)/2 shortest path to be calculated, so the time complexity of this algorithm is (N2).
￼
￼4. Develop environment
Java: >= 1.7. Download from “http://www.oracle.com/ technetwork/java/javase/ downloads/index.html”. 
 
Scala: 2.10.x Should use this version or will cause problems   
Spark: >= 1.3. Download from “http://spark.apache.org/ downloads.html”. When upload java and scala into program, using the command “sbt/sbt assembly” in spark directory, create a jar package named “spark-assembly-***-***.jar” in dictionary “assembly/target/scala-2.10”. 
IDE: Intellij idea. Download from “http://www.jetbrains.com/ idea/”. 
 
4.1 Run program in Intellij idea 
Run this project in local machine in Intellij idea: 
1. Initially, create an usual scala project without SBT. At the first step when building this program, adding Java and scala dependencies as its required as shown below.  
2. When build a project, choose “file -> Project structure”, select “modules- >Dependences->+->Library->Java” adding dependency “spark-assembly-***- ***.jar” as shown below.

While finishing all these settings, load the scala script named “Degree_centrality”. Then, click “Run -> Edit configurations”. In the pop window, choose “+” to adding a application. Choosing the main class to build a run setting. 
￼
￼After that, change the parameter named “path” in the main function of this script to the absolute paths of test files as shown below. Finally, click run.
 
4.2 Create jar package for program 
Click “File-> Project structure”, in the pop window choose “Artifacts”, in the right window press “+ -> JAR” selecting the main class. When these settings have done, choose “Build -> Build Artifacts” to build a jar package for program.

￼
