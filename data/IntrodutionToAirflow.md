# Introdution to Airflow

Apache Airflow is an open-source tool for programmatically authoring, scheduling and monitoring our data pipelines.

# Who Uses Airflow?

    - Data engineers, responsible for build, maintain and manage all data pipelines.
    
    - Data scientists, use to automate the process of pre-processing and analyzing.

    - Data Analyst, use to create SQL queries to dashboardsand reports

    - ML engineers, use to automate processes related to retraining and validating machine learning models.

# Considerations of using Airflow

    - Airflow is designed for batch processing, not for streaming processing.

    - Airflow is scalable by default, you can executeas many task as you want.

    - Airflow is designed for orchestrating and manages data workflows, not process data, is possible process data but is not mainly.

# How does Airflow work?

    DAG (Direct Acyclic Graph)
        
        Directed -> Direction
        
        Acyclic -> Don't have cycle, just one direction.
        
        Graph-> You can define how complex is your graph.
    
    TASK

        A single unit of work in a DAG, represented by a single node in the graph.

    OPERATOR

        The work a task does, serve as the building blocks of DAG's.

    ACTION OPERATORS

        Operator that executes something like postgres to execute SQL requests or python operator, to executes python function.

    TRANSFER OPERATOR

        Transfer data beween source to a destination.

    SENSOR OPERATOR

        Wait for an event before execute the next task.



Resume:

- Data Orchestration is the coordination and automation of data flow across various tools and systems to deliver quality data products and analytics
- The path to modern data orchestration solutions like Airflow had various evolutions starting with basic time-based scheduling tools (e.g., Cron, WTS), followed by proprietary software (e.g., AutoSys, Informatica), and finally older open-source solutions (e.g., Oozie, Luigi).

- Airflow is an open-source tool for programmatically authoring, scheduling, and monitoring data pipelines.
- Airflow is defined by key characteristics such as pipelines-as-code with Python, built-in observability, a large open-source community, and much more!
- Airflow is used across a variety of industries, data practitioners, and use-cases.
- Airflow has key considerations to account for when using it for streaming, data processing, and when it is scaled. 
- Airflow can be used by single developers, single teams, and multi-teams. In each case, the way it is run is different.
- Airflow can be run using a variety of architecture types (e.g., on-premise) and systems (e.g., cloud services)
- Airflow key terms to remember:
    - DAG: A directed acyclical graph that represents a single data pipeline
    - Task: An individual unit of work in a DAG
    - Operator: The specific work that a Task performs 
- There are three main types of operators:
    - Action: Perform a specific action such as running code or a bash command
    - Transfer: Perform transfer operations that move data between two systems
    - Sensor: Wait for a specific condition to be met (e.g., waiting for a file to be present) before running the next task

[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)
