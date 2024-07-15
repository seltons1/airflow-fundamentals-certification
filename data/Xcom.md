# Xcom

- Native feature of Airflow, that enables the sharing of data between tasks by using the Airflow meta database.

- To use XCOM, a DAG and task must first be created, and then an XCOM can be created by returning a value from a task that can be retrieved by another task.
- The XCOM has a key, value, timestamp, task ID, and DAG ID, and must be JSON serializable.

- Using the xcom_push and xcom_pull methods in Airflow, one can define a specific key to an XCOM, giving flexibility in defining task IDs and allowing for pulling data from multiple tasks simultaneously.

- The Airflow UI can display XCOMs and their properties, and XCOMs can be used to share small amounts of metadata between tasks.

- However, XCOMs have limitations based on the database used, with SQLite allowing up to 2GB, Postgres up to 1GB, and MySQL up to 64KB.

- It is not suitable for sharing large amounts of data, and for that, one should trigger a Spark job or similar.

- In summary, XCOMs are a useful feature of Apache Airflow for sharing small amounts of data between tasks, but it is important to understand their limitations and use them accordingly.



[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)