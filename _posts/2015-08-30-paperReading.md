Managing the Academic Data Lifecycle: A Case Study of HPCC

#The summary of the paper: Objectively describe paper without any subjective assessment.

In this research paper the authors introduce the High Performance Computing Cluster (HPCC) as a platform to streamline the process of ingesting, curating, integrating and transforming scholarly data from multiple sources and in varying formats, particularly when several of these datasets lack common attributes to support the integration process.

This paper did a case study of High Performance Computing Cluster(HPCC) in academic data processing. The academic data comes from NSF, NCSES and IPEDS and is in different formats. In the first part, this paper gave a brief discussion of HPCC platform. In the second part, the paper gave a detailed description of the case study in three steps: data ingestion, cleaning and linking data. In the third part, the authors evaluate the performance of HPCC in clusters with different numbers of nodes and discuss HPCC and Hadoop platform.

steps to process data:
data ingestion
cleaning and linking data


#The strengths of the paper: Describe what you believe are the strengths of the paper.
This paper gives detailed description of a HPCC application. It is a good tutorial for HPCC learners.  Take Part 3 for example, it talks a lot about ETL (extract, transform, load) language ,parallel batch data processing (Thor) and high-performance online query applications using indexed data files (Roxie). For HPCC learners, it is good to introduce ETL types and formats like a textbook. Moreover, part 4 discusses the process of HPCC application. It even explains reserved keyword EXPORT in ETL language, which is boring for experts but necessary for learners.
In part 6, the authors discusses the similarities and differences between the Hadoop and HPCC platforms and 

#The weaknesses of the paper: Describe the weakness of the paper in a constructive manner. For example, you may elaborate what the authors could have done to improve the quality of the paper.

The graphs are not clear. For example, graph 1(Thor Cluster) is from wikipedia but missing some explanation. And I am wondering why the authors leave out the Roxie Cluster graph. Graph 9 is confusing because of unclear words. 
The dataset is small and the computation is not much, maybe the example is not good for distributed computing.
Lack analysis of the performance of HPCC under different nodes.
performance and discussion are not closely related .
#The impact of the paper: Assess and elaborate if the paper addresses an important problem in this part.
This paper is a useful search in application of HPCC in academic data , a good start for large academic data.

Give a brief
#The conclusion of your review.

This paper makes a good summary of hpcc application. But the discussion is not so convincing.


#Managing the academic data lifecycle: A case study of HPCC
Payne, Michael E., et al. "Managing the academic data lifecycle: A case study of HPCC." Big Data (Big Data), 2014 IEEE International Conference on. IEEE, 2014.

1.data storage
IPEDS: The Integrated Postsecondary Education Data System
NCSES: National Center for Science and Engineering Statistics
2.HPCC
Thor: the data refinery for cleaning and ETL (extract, transform, load) processing large amounts of data
Roxie (Rapid Online XML Inquiry Engine): the data delivery engine for online high-performance structured querying and analysis.

##The summary of the paper: Objectively describe paper without any subjective assessment.


In this research paper the authors introduce the High Performance Computing Cluster (HPCC) as a platform to streamline the process of ingesting, curating, integrating and transforming scholarly data from multiple sources and in varying formats, particularly when several of these datasets lack common attributes to support the integration process.

##The strengths of the paper: Describe what you believe are the strengths of the paper.
  The part 3 introduces high performance computing cluster including hpcc architecture and enterprise control language, which is good for amature. 
  
#The weaknesses of the paper: Describe the weakness of the paper in a constructive manner. For example, you may elaborate what the authors could have done to improve the quality of the paper.
The graphs in the paper are not clear and concise
  
##The impact of the paper: Assess and elaborate if the paper addresses an important problem in this part.

##The conclusion of your review.


#Draft

Managing the Academic Data Lifecycle: A Case Study of HPCC 
				
This paper did a case study of High Performance Computing Cluster(HPCC) in academic data processing. The academic data comes from NSF(National Science Foundation), NCSES(National Center for Educational Statistics ), National Research Council(NRC), Integrated Postsecondary Education Data System(IPEDS) and other organizations. And the data is in different formats. In the first part, this paper gave a brief discussion of HPCC platform. In the second part, the paper gave a detailed description of the case study in three steps: data ingestion, cleaning and linking data. The paper introduces the content of different datasets. Then Data format including  plain text, CSV, Microsoft Excel and XML is discussed. In this part, Sample ECL code is given to show dataset layout, text cleaning and data transforming function. In the third part, two physical clusters consists of reconfigurable, homogeneous set of nodes are used to test the performance of HPCC .  The execution graph for sample query is given. The result on the first cluster shows that HPCC runs faster for each of the queries as the number of nodes is increased. But the speedup for query 2 and query 3 for a number of nodes beyond two is minimal. In the last part, the paper discusses the development of academic data processing. Also, the paper compare the hardware , data structure, database capability and other factors between HPCC and Hadoop platform.

The paper gives detailed description of a HPCC application. It is a good tutorial for HPCC learners. Take Part 3 for example, it talks a lot about ETL (extract, transform, load) language ,parallel batch data processing (Thor) and high-performance online query applications using indexed data files (Roxie). For HPCC learners, it is good to introduce ETL types and formats like a textbook. Moreover, part 4 discusses the process of HPCC application. It even explains reserved keyword EXPORT in ETL language, which is boring for experts but necessary for learners.

The paper is convincing at giving sample code in part 4: Application of HPCC to scholarly data. The sample code covers data ingestion, transforming, cleaning and linking. In data ingestion, ECL language is used to support CSV, XML, raw text and Excel spreadsheet.  It strongly validates the strengths of HPCC to support unstructured academic data. 

The paper is valuable for discussing the progress in bringing together academic data In part 6.  It reflects the trend of academic data storage selection from SQL to No-SQL.  The need to employ data-intensive computing is brought out. Also,The authors discusses the similarities and differences between the Hadoop and HPCC platforms.

However, the paper suffers several drawbacks. There is one big issue about the meaning of using HPCC. The dataset is the order of several GBs. Why should we use HPCC instead of personal computer? The dataset is small (can be stored in 16GB of RAM) and the computation is not much, maybe the example is not good for distributed computing.  For example, the paper says that the HPCC standard library(Str library and machine learning library) makes data cleaning easier. But there are other python library(like re) to do the same work. The paper should give strong evidence of the benefit of HPCC. Also, the experiment on two clusters are not comparable because the memory of each node in different cluster is varying. Why doesn’t the paper replicate the same queries on the same cluster?  Moreover, it is confusing to compare HPCC and Hadoop in the discussion part. The paper did a case study of HPCC and the experiment and performance evaluation is done in HPCC framework. The result doesn’t include Hadoop performance. So the comparison is not based on experiment result and unreliable. 
Except from the above two issues, there are some weakness in the writing and organization.
The graphs are not clear. For example, graph 1(Thor Cluster) is from wikipedia but missing some explanation. The paper doesn’t give the reason why it leaves out the Roxie Cluster graph. Graph 9 is confusing because of bad layout and unclear numbers on the line.
Lack analysis of the performance of HPCC under different nodes. performance and discussion are not closely related .
Abbreviations like NCSES are confusing because the paper doesn’t give the full name when they are firstly mentioned.
There are grammar mistakes. For example, the first sentence of Part 5: “Two physical clusters are used test the performance performance of HPCC” should be changed as “ Two physical clusters are used to test the performance of HPCC”. 

To evaluate the value of the paper, it is a useful investigation in application of HPCC in academic data , a good start for processing large academic data. Firstly, it brings out an interesting problem: processing and integrating a large amount of academic data under various formats from various sources without any consistency or a predefined data structure. A comprehensive platform to support the entire academic data lifecycle is needed in the future.   Secondly, it gave a solution of HPCC framework to solve the computing problem. The details of HPCC framework and ECL code implementation are included in the paper. It is a good tutorial for HPCC learners who are interested in used HPCC framework to solve similar problem. It also supports basic standard for academic data processing in distributed system.  However, the data set is too small to be considered as “big data”. In the experiment, query performance result on one node is hundreds of seconds. It is not good for real time query, but it is fast enough to generate a report for government or policy makers mentioned in the abstract. So the paper should better claim why we should use HPCC instead of other architectures to compute academic data. Is the academic data expanding very large in the future? Or the requirement of real-time query is essential? By answering these doubts, the paper can make the solution of HPCC framework more valuable. What’s more, it is better to fix those graph and grammar mistakes in the paper. There are similar papers of case study in this field. For example, [1-2] are better at supplying new methodology in different situation. Liu [1] proposed an approach to optimize I/O performance of small files on HDFS. It is a better case study because it summarizes a certain kind of problem from WebGIS data.
In summary, the paper makes a brief introduction to HPCC and did a case study of HPCC framework in academic data manipulating. It is an good tutorial for case study of HPCC and the process can be replicated in other case studies. But it is not a very good paper to be read for many times. There is no breakthrough methodology in the paper. The experiment and the discussion are not closely related. The grammar mistakes undermine the value of the paper. After all, it can not a classic paper.

[1] Liu, Xuhui, et al. "Implementing WebGIS on Hadoop: A case study of improving small file I/O performance on HDFS." Cluster Computing and Workshops, 2009. CLUSTER'09. IEEE International Conference on. IEEE, 2009.
[2] Papadimitriou, Spiros, and Jimeng Sun. "Disco: Distributed co-clustering with map-reduce: A case study towards petabyte-scale end-to-end mining." Data Mining, 2008. ICDM'08. Eighth IEEE International Conference on. IEEE, 2008.


