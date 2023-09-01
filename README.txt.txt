Project Information

Title: Word Count and Analysis in Plain Text File

Summary: 
 - Perform data engineering and analysis on info_tech.txt file by using Apache Spark framework to 
   1. determine the number of times each word appears in the file and then write the output to DBFS storage 
   2. fetch all the rows in the file that contain the string "information technology" and then write the same to DBFS storage 

Data File Details:
 - The file info_tech.txt is an expository write-up on importance of Information Technology to students
 - File size : 5 KB
 - Data Source : Windows PC

Data Cleaning Requirements: None

Methodology: 
 - Upload info_tech.txt file to DBFS storage from the local machine
 - Read info_tech.txt data into spark notebook for transformation and analysis
 - Count the number of appearances for each word, store the output in a dataframe, df_word_count and then write the dataframe to DBFS storage as 'count.parquet' file
 - Fetch all the rows in the file that contain the string "information", store the output in a dataframe, df_info and then write 
   the dataframe to DBFS storage as 'information.parquet' file
 - Fetch all the rows in the df_info that contain the string "technology", store the output in a dataframe, df_info_tech and then write 
   the dataframe to DBFS storage as 'information_technology.parquet' file

Tech Stack:
 - Databricks (Community Edition)

Languages/Runtimes
 - Apache Spark 3.3.2


 