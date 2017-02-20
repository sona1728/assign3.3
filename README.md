*Hadoop 2.x has the following three Major Components:
1. HDFS
2. YARN
3. MAPREDUCE

- These three are also known as Three Pillars of Hadoop 2.x. Here major key component change is YARN. It is really game changing component in BigData Hadoop System.

#Hadoop Distributed File System (HDFS):

- The default big data storage layer for Apache Hadoop is HDFS. HDFS is the “Secret Sauce” of Apache Hadoop components as users can dump huge datasets into HDFS and the data will sit there nicely until the user wants to leverage it for analysis. 
- HDFS component creates several replicas of the data block to be distributed across different clusters for reliable and quick data access. HDFS comprises of 3 important components-NameNode, DataNode and Secondary NameNode.
- HDFS operates on a Master-Slave architecture model where the NameNode acts as the master node for keeping a track of the storage cluster and the DataNode acts as a slave node summing up to the various systems within a Hadoop cluster.

#YARN:

- YARN forms an integral part of Hadoop 2.0.YARN is great enabler for dynamic resource utilization on Hadoop framework as users can run various Hadoop applications without having to bother about increasing workloads.

-Key Benefits of Hadoop 2.0 YARN Component:

- It offers improved cluster utilization.
- Highly scalable.
- Beyond Java.
- Novel programming models and services.
- Agility.

#MAPREDUCE:

- MapReduce is a Java-based system created by Google where the actual data from the HDFS store gets processed efficiently. MapReduce breaks down a big data processing job into smaller tasks.
- MapReduce is responsible for the analysing large datasets in parallel before reducing it to find the results. In the Hadoop ecosystem, Hadoop MapReduce is a framework based on YARN architecture.
- YARN based Hadoop architecture, supports parallel processing of huge data sets and MapReduce provides the framework for easily writing applications on thousands of nodes, considering fault and failure management.
- The basic principle of operation behind MapReduce is that the “Map” job sends a query for processing to various nodes in a Hadoop cluster and the “Reduce” job collects all the results to output into a single value.
- Map Task in the Hadoop ecosystem takes input data and splits into independent chunks and output of this task will be the input for Reduce Task.
- MapReduce takes care of scheduling jobs, monitoring jobs and re-executes the failed task.

#WORKING OF COMPONENTS OF HADOOP 2.x:

- Hadoop 2.x components follow this architecture to interact each other and to work parallel in a reliable, highly available and fault-tolerant manner.
- All Master Nodes and Slave Nodes contains both MapReduce and HDFS Components.

-One Master Node has two components:
1. Resource Manager(YARN or MapReduce v2)
2. HDFS

- It’s HDFS component is also knows as NameNode. It’s NameNode is used to store Meta Data.

- In Hadoop 2.x, some more Nodes acts as Master Nodes. Each this 2nd level Master Node has 3 components:
1. Node Manager
2. Application Master
3. Data Node

- Each this 2nd level Master Node again contains one or more Slave Nodes as shown in the above diagram.
- These Slave Nodes have two components:
1. Node Manager
2. HDFS

- It’s HDFS component is also knows as Data Node. It’s Data Node component is used to store actual our application Big Data. These nodes does not contain Application Master component

FOR ARCHITECTURE: REFER THE FILE UPLOADED.
