# Opening ....
目前服務是使用databricks，一併來進行databricks certification。

## 例題QA
Question #2
```
Q: Which of the following describes a scenario in which a data team will want to utilize cluster pools?
A. An automated report needs to be refreshed as quickly as possible.
```
Note: [Databricks Pools](
https://www.databricks.com/blog/2019/11/11/databricks-pools-speed-up-data-pipelines.html)


Question #3
```
Q: Which of the following is hosted completely in the control plane of the classic Databricks architecture?
A: Databricks web application
```

Question #4
```
Q: Which of the following benefits of using the Databricks Lakehouse Platform is provided by Delta Lake?
A: The ability to support batch and streaming workloads 
```
Note: *** [What is Delta Lake](https://learn.microsoft.com/en-us/azure/databricks/delta/)

Learn:
Delta Lake是一個基於Parquet的優化儲存層，具備以下特點:
- 開源
- 支援ACID
- 可擴展的元數據管理
- 全支援 Spark API
- 專門為了整合流處理而開發

Question #5
```
Q: Which of the following describes the storage organization of a Delta table?
A: Delta tables are stored in a collection of files that contain data, history, metadata, and other attributes.
```

Question #7
```
Q: A data engineer has realized that they made a mistake when making a daily update to a table. They need to use Delta time travel to restore the table to a version that is 3 days old. However, when the data engineer attempts to time travel to the older version, they are unable to restore the data because the data files have been deleted.
Which of the following explains why the data files are no longer present?
A: The VACUUM command was run on the table
```

Question #9
```
Q: Which of the following data lakehouse features results in improved data quality over a traditional data lake?
A: A data lakehouse supports ACID-compliant transactions.
```

Question #10
```
Q: A data engineer needs to determine whether to use the built-in Databricks Notebooks versioning or version their project using Databricks Repos.
Which of the following is an advantage of using Databricks Repos over the Databricks Notebooks versioning?
A: Databricks Repos supports the use of multiple branches
```

Question #11
```
Q: A data engineer has left the organization. The data team needs to transfer ownership of the data engineer’s Delta tables to a new data engineer. The new data engineer is the lead engineer on the data team.
Assuming the original data engineer no longer has access, which of the following individuals must be the one to transfer ownership of the Delta tables in Data Explorer?
A: Workspace administrator
```

Question #12
```
Q: A data analyst has created a Delta table sales that is used by the entire data analysis team. They want help from the data engineering team to implement a series of tests to ensure the data is clean. However, the data engineering team uses Python for its tests rather than SQL.
Which of the following commands could the data engineering team use to access sales in PySpark?
A: spark.table("sales")
```

Question #13
```
Q: Which of the following commands will return the location of database customer360?
A: DESCRIBE DATABASE customer360
```

Question #14
```
Q: A data engineer wants to create a new table containing the names of customers that live in France.
They have written the following command:
Which of the following lines of code fills in the above blank to successfully complete the task?
A: COMMENT "Contains PII"
```

Question #15
```
Q: Which of the following benefits is provided by the array functions from Spark SQL?
A: An ability to work with complex, nested data ingested from JSON files
```

Question #17
```
Q: A data engineer needs to apply custom logic to string column city in table stores for a specific use case. In order to apply this custom logic at scale, the data engineer wants to create a SQL user-defined function (UDF).
Which of the following code blocks creates this SQL UDF?
A: 
CREATE FUNCTION plus(a INT, b INT)
RETURNS INT
RETURN CASE
        WHEN a = 0 AND b > 0 THEN b
        WHEN a > 0 AND b = 0 THEN a
        ELSE a+b
END
;     
```

Question #18
```
Q: A data analyst has a series of queries in a SQL program. The data analyst wants this program to run every day. They only want the final query in the program to run on Sundays. They ask for help from the data engineering team to complete this task.
Which of the following approaches could be used by the data engineering team to complete this task?
A: They could wrap the queries using PySpark and use Python’s control flow system to determine when to run the final query.
```

Question #19
```
Q: A data engineer runs a statement every day to copy the previous day’s sales into the table transactions. Each day’s sales are in their own file in the location "/transactions/raw".
Today, the data engineer runs the following command to complete this task:
After running the command today, the data engineer notices that the number of records in table transactions has not changed.
Which of the following describes why the statement might not have copied any new records into the table?
A: The previous day’s file has already been copied into the table.
```


## referance:
- 報名網址: [Databricks Certified Data Engineer Associate](https://www.databricks.com/learn/certification/data-engineer-associate)

- 例題討論: [ExamTopics](https://www.examtopics.com/exams/databricks/certified-data-engineer-associate/)

- 推薦課程: (https://www.udemy.com/share/10aEFa3@9M_uT6vrKbnl68tOK96kfy-YWitjwzLTlVCrzPs-0hGUu8fyX8V4Tn_x_y65bwLm/)
