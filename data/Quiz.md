# Quiz

# 1. Introdution to Orchestration and Airflow
Question 1:

Which of the following describes the pre-unix era of Data Orchestration? (select all that apply)

    Automated Processes
    Dedicated ETL tooling
    (True) Lack of standards around data formats, processes, and processing techniques
    (True) Manual and error-prone processes

Question 2:

Which of the following describes the data and open-source era of Data Orchestration? (select all that apply)

    (True) Tools that were designed for specific ecosystems (e.g., Hadoop)
    (True) An increase in data size and complexity of scheduling and workloads
    Adoption of proprietary data formats and protocols to restrict access to data ecosystems
    Manual batch processing

Question 3: 

Which of the following describes the early-computing era of Data Orchestration? (select all that apply)

    Lack of standards around data formats, processes, and processing techniques
    (True) Rise of proprietary scheduling and workload management tools (e.g., AutoSys)
    Manual processes
    (True) Time-based scheduling tools (e.g., Cron)

Question 4:

Which of the following is the definition of modern data orchestration?

    (True) The coordination and automation of data flow across various tools and systems to deliver quality data products and analytics.
    The exclusive use of a single tool to manage all data-related tasks within an organization.
    The random distribution and storage of data across various databases without any automated processes.
    The process of manually handling data flow across different platforms to ensure data security and compliance.

________________________________________________________________

Question 1:

Why is Airflow considered the central nervous system of a data stack?

    (True) It connects, coordinates, and manages different tools and systems across a organization's data ecosystem
    It provides data storage solutions for large datasets.
    It functions as a data visualization platform.
    It acts as a standalone tool for data analysis

Question 2: 

Fill in the blank: 

Airflow is an open-source tool for programmatically authoring, scheduling, and monitoring ____.

    Answer: "data pipelines" or "data workflows" 

Question 3: 

Which of the following are characteristics of Airflow? (select all that apply)

    (True) The ability to write pipelines-as-code with Python
    Proprietary and closed-source
    (True) Extensibility to connect to external systems
    (True) Built-in observability features

________________________________________________________________


Question 1: 

Which of the following data practitioner personas would most likely use Airflow to productionize SQL queries to create dashboards and reports?

    Machine Learning Engineers
    (True) Data Analysts
    Data Engineers
    Data Scientists

Question 2:

Which of the following data practitioner personas would most likely use Airflow to automate processes related to retraining and validating machine learning models?

    Data Analysts
    (True) Machine Learning Engineers
    Data Scientists
    Data Engineers

Question 3: 

Which of the following data practitioner personas would most likely use Airflow to automate the process of pre-processing and analyzing new data sets?

    Data Analysts
    Data Engineers
    (True) Data Scientists
    Machine Learning Engineers

Question 4: 

Imagine that you are working for a startup that wants to streamline customer support by creating an AI chatbot that would give tips and solutions based on customer errors and actions. Is this a use case for Airflow?

    No
    (True) Yes

Question 5: 

Which of the following data practitioner personas would most likely be primarily responsible for using Airflow to build, maintain, and manage most or all data pipelines for an organization? 

    Machine Learning Engineers
    Data Scientists
    (True) Data Engineers
    Data Analysts

____________________________________________________________________________


Question 1: 

Which of the following would most likely be the root cause of errors when using Airflow for data processing? (select all that apply)

    (True) Resource allocation
    (True) Infrastructure
    A dedicated streaming solution (e.g., Apache Kafka) integrated with Airflow
    Number of data pipelines created

Question 2: 

Which of the following statements are true about Airflow? (select all that apply)

    (True) Airflow is a scalable solution for data orchestration
    Airflow was designed to be used as a dedicated streaming system
    (True) Airflow can preform data processing

Question 3: 

Fill in the blank: 

Airflow was designed to be used for _______ and not streaming.
    
    (True) batch processing

___________________________________________________________________________________________


Question 1: 

Which of the following are most likely the main requirements for running Airflow for production as a single developer? (select all that apply)

    Multi-tenancy
    High levels of scalability
    (True) Low infrastructure overhead
    (True) Low cost

Question 2: 

Which of the following are most likely the main requirements for running Airflow for production in a multi-team environment? (select all that apply)

    Low cost
    (True) High availability
    (True) Scalability
    (True) Multi-tenancy

Question 3:

Which of the following are the most likely ways Airflow will be run in production by a single team? (select all that apply)

    On a single developers machine
    (True) On a fully-managed Airflow service (e.g., Astro)
    (True) On cloud virtual machines (e.g., EC2)
    (True) On a container cloud offering (e.g., EKS)

Question 4: 

Which of the following is the most likely way a developer or team is going to run Airflow if they have to adhere to strict security or regulatory guidelines?

    On a single developers machine
    On a cloud software
    (True) On-premise

    Question 5: 

Which of the following is the most likely way a solo developer will run Airflow for the purposes of experimentation and learning?
    
    On a paid cloud virtual machine (VM) service (e.g., EC2)
    (True) On a local machine or a free virtual machine (VM)
    On a highly secure on-premises architecture
    On a multi-deployment cloud solution (e.g., EKS)

____________________________________________________________________________________________


Question 1:

Which of the following are characteristics of a Airflow DAG? (select all that apply)

    Cyclical
    (True) Graph based
    (True) Composed of Tasks
    (True) Directed
    Represents multiple data pipelines

Question 2:

What is a task in Airflow?

    (True) A single unit of work in a DAG
    The entire data pipeline
    A configuration file for how Airflow is setup on a machine
    The direction the data pipeline executes

Question 3: 

Assume you are building a DAG and want to wait for a file to load before executing the next task. What type of Operator would you use to accomplish this goal?

    (True) Sensor Operator
    Transfer Operator
    Action Operator
    There are no Operators that allow a DAG to wait for something to load

Question 4: 

Assume you are building a DAG and want to move data from one system or data source to another. What type of Operator would you use to accomplish this goal?

    Action Operator
    (True) Transfer Operator
    Sensor Operator
    There are no Operators that allow a DAG to move data from one system or data source to another

Question 5:

Fill in the blank: 

In Airflow, an Operator is the specific work a _____ does.

    (True) task

Question 6:

Assume you are building a DAG and want to run a Python script. What type of Operator would you use to accomplish this goal?

    There are no Operators that allow a DAG to run a Python script
    Sensor Operator
    Transfer Operator
    (True) Action Operator

____________________________________________________________________________________________

Question 1: 

Examine the diagram of a data pipeline in Airflow below: 

Each letter label represents a key term to describe the associated component of the data pipeline. Which of the following is the correct labeling of each component? 

    (True) A) DAG B) Task C) Operator
    A) Task B) DAG C) Operator
    A) Task B) Operator C) DAG
    A) Operator B) Task C) DAG

Question 2: 

Examine the data orchestration diagram below: 

The diagram has the following labeled processes:

    A) Data ingestion of data sources
    B) Creating analytics and reporting
    C) Creating new data sets and data products
    D) Using MLFlow to productionize and manage predictive models

Which of the following best matches each data practitioner persona to each process in the diagram?

    A) ML Engineer B) Data Engineer C) Data Scientist D) Data Analyst
    A) Data Engineer B) Data Scientist C) Data Analyst D) ML Engineer
    (True) A) Data Engineer B) Data Analyst C) Data Scientist D) ML Engineer
    A) Data Scientist B) Data Engineer C) ML Engineer D) Data Analyst

Question 3: 

Which of the following scenarios would be a valid use-case for Airflow? (select all that apply)

    (True) Periodic analysis on sensor data from manufacturing equipment to forecast potential failures and schedule maintenance automatically
    As a dedicated system for processing real-time, high-volume data streams for a stock trading application
    (True) A health care application that schedules email reminders for patients for their appointments
    (True) An AI chatbot that gives tips and solutions based on customer errors and actions

Question 4: 

The benefits of using a modern data orchestration tool like Airflow is because it offers the ability to...(select all that apply)

    (True) Integrate with hundreds of external systems/software
    (True) Schedule data based on events in addition to time
    Author pipelines as configuration files
    (True) Use a rich feature set with features like built-in observability
    Store, secure and preserve large quantities of data permanently


# 2. Airflow Basics

Airflow core componemts

Question 1:

Fill in the blank: 

The core component of Airflow that serves and updates the user interface is the _____.

    web server

Question 2: 

Which of the following best describes the role of an executor in Airflow?

    (True) To determine how and where tasks are executed
    To visualize the pipeline runs
    To execute the instructions of tasks
    To store tasks ready to be executed

Question 3: 

Which of the following best describes the role of the scheduler in Airflow? 

    To store metadata about the state of tasks
    To execute the instructions defined in tasks
    (True) To determine which tasks need to be executed and when
    To define connections to external systems (e.g., Data Warehouses)

Question 4: 

Which Airflow component is in charge of executing the logic of a DAG's tasks?

    (True) The worker
    The scheduler
    The executor
    The metadata database

___________________________________________________________________________________________________

How does airflow run a DAG?

Question 1:  

Fill in the blank:

The Airflow scheduler scans for new tasks to run every 5 seconds from the ______.

    meta database

Question 2:  

After creating your DAG in a Python file, which action do you need to take in order for Airflow to start the process of detecting and running your DAG?

    (True) Put the Python file in the dags directory
    Launch the Airflow web server
    Wait for the scheduler to pick up the tasks defined in the DAG
    Restart Airflow and make sure the DAG is visible on the UI

Question 3:  

When does the metadata database communicate with the other Airflow components?

    Only when a DAG is starting to run
    Only when a DAG is finished running
    (True) Throughout the entire process of running a DAG

Question 4:

The list below summarizes the first four steps of the process of Airflow running a DAG, with the third step missing. 

1. The Airflow scheduler detects a new DAG in the DAGs directory
2. The Airflow scheduler serializes the the DAG and stores it in the metadata database
3. ?
4. The scheduler sends the DAG's tasks into the executors queue

What would happen in step 3? 

    The worker pull the tasks from the queue
    (True) The Airflow scheduler scans the metadata database to see if any DAGs are ready to run
    The metadata database scans the new DAG for any issues
    The workers run the instructions defined in the tasks

Question 5:  

By default, how long can it take for the Airflow scheduler to detect a new DAG file in the dags directory?

    1 minute
    30 seconds
    5 seconds
    (True) 5 minutes


___________________________________________________________________________________________________



DAG setup

Question 1:

Assume you had a DAG with two tasks: task_one and task_two. The dependency defined in the DAG for these two tasks is: 

task_one >> task_two

Fill in the blank below to correctly describe the dependency relationship: 

task_one is _____ to task_two.

    Answer: "Upstream"

Question 2: 

Examine the following code:

from airflow import DAG
from airflow.operators.python_operator import PythonOperator

In your own words, what does this code do?
Your response:
Realize imports to identify that file is a DAG

Question 3: Correct answer

In which part of a DAG file would you specify how often you want to trigger the DAG?

    In the import statements
    In the DAG's tasks
    (True) In the DAG object definition
    In the DAG's dependencies


___________________________________________________________________________________________________


Question 1: 

Which of the following Airflow components does the metadata database communicate with? 

    (True) The webserver
    (True) The worker(s)
    The queue
    (True) The scheduler

Question 2: 

Assume a DAG has 3 tasks: ta, tb, and tc. You want the DAG to execute each task, one after the other, starting with ta, then tb, and finally tc.

Fill in the blank below to correctly define the dependencies of the DAG using either the right (>>) or the left (<<) bitshift operators to reflect the order stated above.

Note: Make sure to include spaces between each task and bitshift operator like so: 
t1 >> t2

    ta >> tb >> tc

Question 3:

Which of the following fills in the following sentence blanks correctly? 

Once a DAG is ready to run, the __________ sends the tasks to the __________. Once a __________ is available, the instructions defined in the task are executed. During the process, the __________ is updated with the DAGs changing state.

    Queue, Metadata Database, Scheduler, Worker
    Scheduler, Worker, Queue, Metadata Database
    Metadata Database, Queue, Worker, Scheduler
    Metadata Database, Queue, Scheduler, Worker
    (True) Scheduler, Queue, Worker, Metadata Database

Question 4:

Assume a DAG has 3 tasks: task_extract, task_transform, and task_load.

Which of the following represents the dependencies in a DAG that needs to meet the following conditions:

task_transform is downstream of task_extract.
task_load is downstream of task_transform.

    (True) task_extract >> task_transform >> task_load
    task_extract << task_load << task_transform
    task_extract >> task_load >> task_transform

# 3. Local Development Environment