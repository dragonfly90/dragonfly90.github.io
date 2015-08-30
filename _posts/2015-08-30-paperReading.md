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
