# Introdution to Airflow

Apache Airflow is an open-source tool for programmatically authoring, scheduling and monitoring our data pipelines.

# Who Uses Airflow?

    - Data engineers, responsible for build, maintain and manage all data pipelines.
    
    - Data scientists, use to automate the process of pre-processing and analyzing.

    - Data Analyst, use to create SQL queries to dashboardsand reports

    - ML engineers, use to automate processes related to retraining and validating machine learning models.

# Considerations of using Airflow

    - Airflow is designed for batch processing, not for streaming processing.

    - Airflow is scalable bu default, you can executeas many task as you want.

    - Airflow is designed for orchestrating and manages data workflows, not process data, is possible process data but is not mainly.

# How does Airflow work?

    DAG (Direct Acyclic Graph)
        
        Directed -> Direction
        
        Acyclic -> Don't have cycle, just one direction.
        
        Graph-> You can define how complex is your graph.
    
    TASK

        A single unit of work in a DAG, represented by a single node inthe graph.

    OPERATOR

        The work a task does, serve as the building blocks of DAG's.

    ACTION OPERATORS

        Operator that executes something like postgres to execute SQL requests or python operator, to executes python function.

    TRANSFER OPERATOR

        Transfer data beween source to a destination.

    SENSOR OPERATOR

        Wait for an event before execute the next task.


[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)