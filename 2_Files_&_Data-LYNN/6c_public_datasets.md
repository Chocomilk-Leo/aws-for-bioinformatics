# Athena SQL Datasets & More Query Info

### Why do this
 - **Learn** SQL query concepts so that you can use AWS Big Query service using your own version of my source data (CSV files)
 - **Practice** SQL query concepts by writing & executing queries against Athena datasets

### Create your own example Athena Dataset

 If you want to set up your own copy of the example Athena dataset, use the CSV files provided [in this Repository](https://github.com/lynnlangit/AWS-for-bioinformatics/tree/master/1_Files_%26_Data/genomic-data-samples/CSV-or-TXT/CSV-for-Athena-lessons)
  - GET your source files or use my CSV files
  - OPEN each CSV files to... 
    - review/update the file structure 
    - review/update the data 
    - SAVE each file
  - CREATE a Athena dataset using the Web UI
    - CREATE one Athena table for each CSV file inside of your BQ Dataset
      - To create table schema
        - enter each column name and data type manually --or-- 
        - use Athena 'auto-detect' table schema IF all of the following conditions are met:
          - DELIMETERS - your source files use tab, comma or pipe delimeters 
          - DATA TYPES - each file must have at least one non-string column, i.e. integer, float, date
          - HEADERS - you can set to skip 1 row if your source data has headers
          - WHITE SPACE (in string data type columns)Athena INCLUDES all white space in string fields, so if you want to remove that white space you must remove it in the source file before you create your Athena tables

Review the example Athena dataset schema and example data (graphic below)

  [![SQL example schema](/images/sql-data-model.png)]()

### How to verify you've done it
 - View the dataset in your Athena tree (see below)
 - Click on each table to verify schema and data

[![BQ Dataset](/images/bq-dataset.png)]()

### Other Things to Know
 - Your BQ dataset is set by default to only be accessible by you within your AWS project.  If you want to make this dataset available to other AWS others, then you must manually set the access permissions on your BQ dataset.
 - SQL is a set-based query language for data tables 
 - Joining table rows is a key concept. The graphic below shows join concepts

[![SQL Keywords](/images/joins.png)]()

### How to learn more
 - 📘 Link to [learn SQL - 12 questions](https://en.wikibooks.org/wiki/Data_Management_in_Bioinformatics/SQL_Exercises)
 - 📘 Link to [standard SQL syntax](https://cloud.google.com/Athena/docs/reference/standard-sql/query-syntax) used in Google Athena  
  - 📘 Link to [example genomics SQL queries](https://codelabs.developers.google.com/codelabs/genomics-vcfbq/#4) shown using Google Athena
 - 📘 Link to [learn SQL - 12 questions](https://en.wikibooks.org/wiki/Data_Management_in_Bioinformatics/SQL_Exercises)
 - 📘 Link to [standard SQL syntax](https://cloud.google.com/Athena/docs/reference/standard-sql/query-syntax) used in Google Athena  
  - 📘 Link to [example genomics SQL queries](https://codelabs.developers.google.com/codelabs/genomics-vcfbq/#4) shown using Google Athena 
 
 