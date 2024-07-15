# Variables

Variables are very useful to not duplicated code, you can define a variable that can use in all tasks, like a global variable.

- The use of variables in programming can simplify and streamline code by storing information that can be used across multiple tasks or functions. Variables consist of a unique identifier, a value that is JSON serializable.

- They can be created, edited, deleted, or exported and can also be stored in a secret backend or by using environment variables.
For sensitive values, Airflow allows for the creation of hidden variables by specifying certain keywords such as "api_key", "password", or "secret" in the key. These variables remain hidden on the Airflow UI even when edited, providing a safe way to store sensitive information.

- In addition, Airflow variables can be created by exporting environment variables with the prefix "AIRFLOW_VAR". This method allows for keeping sensitive values hidden from the Airflow UI, faster processing, and easy versioning of variables as they are stored in a file.

- While these variables cannot be seen on the Airflow UI, they can still be used in DAGs.

- Overall, the use of variables in Airflow can simplify code, improve efficiency, and provide a safe way to store sensitive information.


[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)