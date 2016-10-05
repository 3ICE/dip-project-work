# Coursework for TIE-22306 Data-Intensive Programming
##by Daniel "3ICE" Berezvai, Arjun Venkat, and Juho Peltonen

###Task 1 & 2:
####What are the top-10 best selling products in terms of total sales? & What are the top-10 browsed products?
 * flume-config
 * run-flume.sh
 * ProductCount.java
   - Regex used: https://regex101.com/r/eDt96O/1
   - **TESTING**: Run/Debug configuration → Program arguments: `/home/hduser/Desktop/log-data/ out2`
   - **PRODUCTION**: Compile and then execute with `hadoop jar productcount.jar fi.tut.ProductCount log-data out2`
 * SampleOutput.txt
 * psql
 
 
###Task 3:
####What anomaly is there between these two?
/ToDo/

###Task 4:
####What are the most popular browsing hours?
/ToDo/

##Guidelines
Since the managers of the company don’t use Hadoop but a RDBMS, all the data must be transferred to PostgreSQL. Therefore, the detailed tasks are:
* Transfer Apache logs (with Apache Flume) to the HDFS
* Compute the frequencies of viewing of different products using MapReduce (Question 2)
* Compute the viewing hour data with MapReduce (Q4)
* Transfer the results (with Apache Sqoop) to PostgreSQL
* Find answer to the questions in PostgreSQL using SQL (Q1-4)