# Quiz

# 1. Introdution to Orchestration and Airflow


Which of the following describes the pre-unix era of Data Orchestration? (select all that apply)

    Automated Processes
    Dedicated ETL tooling
    (True) Lack of standards around data formats, processes, and processing techniques
    (True) Manual and error-prone processes



Which of the following describes the data and open-source era of Data Orchestration? (select all that apply)

    (True) Tools that were designed for specific ecosystems (e.g., Hadoop)
    (True) An increase in data size and complexity of scheduling and workloads
    Adoption of proprietary data formats and protocols to restrict access to data ecosystems
    Manual batch processing

 

Which of the following describes the early-computing era of Data Orchestration? (select all that apply)

    Lack of standards around data formats, processes, and processing techniques
    (True) Rise of proprietary scheduling and workload management tools (e.g., AutoSys)
    Manual processes
    (True) Time-based scheduling tools (e.g., Cron)



Which of the following is the definition of modern data orchestration?

    (True) The coordination and automation of data flow across various tools and systems to deliver quality data products and analytics.
    The exclusive use of a single tool to manage all data-related tasks within an organization.
    The random distribution and storage of data across various databases without any automated processes.
    The process of manually handling data flow across different platforms to ensure data security and compliance.

________________________________________________________________



Why is Airflow considered the central nervous system of a data stack?

    (True) It connects, coordinates, and manages different tools and systems across a organization's data ecosystem
    It provides data storage solutions for large datasets.
    It functions as a data visualization platform.
    It acts as a standalone tool for data analysis

 

Fill in the blank: 

Airflow is an open-source tool for programmatically authoring, scheduling, and monitoring ____.

    Answer: "data pipelines" or "data workflows" 

 

Which of the following are characteristics of Airflow? (select all that apply)

    (True) The ability to write pipelines-as-code with Python
    Proprietary and closed-source
    (True) Extensibility to connect to external systems
    (True) Built-in observability features

________________________________________________________________


 

Which of the following data practitioner personas would most likely use Airflow to productionize SQL queries to create dashboards and reports?

    Machine Learning Engineers
    (True) Data Analysts
    Data Engineers
    Data Scientists



Which of the following data practitioner personas would most likely use Airflow to automate processes related to retraining and validating machine learning models?

    Data Analysts
    (True) Machine Learning Engineers
    Data Scientists
    Data Engineers

 

Which of the following data practitioner personas would most likely use Airflow to automate the process of pre-processing and analyzing new data sets?

    Data Analysts
    Data Engineers
    (True) Data Scientists
    Machine Learning Engineers

 

Imagine that you are working for a startup that wants to streamline customer support by creating an AI chatbot that would give tips and solutions based on customer errors and actions. Is this a use case for Airflow?

    No
    (True) Yes

 

Which of the following data practitioner personas would most likely be primarily responsible for using Airflow to build, maintain, and manage most or all data pipelines for an organization? 

    Machine Learning Engineers
    Data Scientists
    (True) Data Engineers
    Data Analysts

____________________________________________________________________________


 

Which of the following would most likely be the root cause of errors when using Airflow for data processing? (select all that apply)

    (True) Resource allocation
    (True) Infrastructure
    A dedicated streaming solution (e.g., Apache Kafka) integrated with Airflow
    Number of data pipelines created

 

Which of the following statements are true about Airflow? (select all that apply)

    (True) Airflow is a scalable solution for data orchestration
    Airflow was designed to be used as a dedicated streaming system
    (True) Airflow can preform data processing

 

Fill in the blank: 

Airflow was designed to be used for _______ and not streaming.
    
    (True) batch processing

___________________________________________________________________________________________


 

Which of the following are most likely the main requirements for running Airflow for production as a single developer? (select all that apply)

    Multi-tenancy
    High levels of scalability
    (True) Low infrastructure overhead
    (True) Low cost

 

Which of the following are most likely the main requirements for running Airflow for production in a multi-team environment? (select all that apply)

    Low cost
    (True) High availability
    (True) Scalability
    (True) Multi-tenancy



Which of the following are the most likely ways Airflow will be run in production by a single team? (select all that apply)

    On a single developers machine
    (True) On a fully-managed Airflow service (e.g., Astro)
    (True) On cloud virtual machines (e.g., EC2)
    (True) On a container cloud offering (e.g., EKS)

 

Which of the following is the most likely way a developer or team is going to run Airflow if they have to adhere to strict security or regulatory guidelines?

    On a single developers machine
    On a cloud software
    (True) On-premise

     

Which of the following is the most likely way a solo developer will run Airflow for the purposes of experimentation and learning?
    
    On a paid cloud virtual machine (VM) service (e.g., EC2)
    (True) On a local machine or a free virtual machine (VM)
    On a highly secure on-premises architecture
    On a multi-deployment cloud solution (e.g., EKS)

____________________________________________________________________________________________




Which of the following are characteristics of a Airflow DAG? (select all that apply)

    Cyclical
    (True) Graph based
    (True) Composed of Tasks
    (True) Directed
    Represents multiple data pipelines



What is a task in Airflow?

    (True) A single unit of work in a DAG
    The entire data pipeline
    A configuration file for how Airflow is setup on a machine
    The direction the data pipeline executes

 

Assume you are building a DAG and want to wait for a file to load before executing the next task. What type of Operator would you use to accomplish this goal?

    (True) Sensor Operator
    Transfer Operator
    Action Operator
    There are no Operators that allow a DAG to wait for something to load

 

Assume you are building a DAG and want to move data from one system or data source to another. What type of Operator would you use to accomplish this goal?

    Action Operator
    (True) Transfer Operator
    Sensor Operator
    There are no Operators that allow a DAG to move data from one system or data source to another



Fill in the blank: 

In Airflow, an Operator is the specific work a _____ does.

    (True) task



Assume you are building a DAG and want to run a Python script. What type of Operator would you use to accomplish this goal?

    There are no Operators that allow a DAG to run a Python script
    Sensor Operator
    Transfer Operator
    (True) Action Operator

____________________________________________________________________________________________

 

Examine the diagram of a data pipeline in Airflow below: 

Each letter label represents a key term to describe the associated component of the data pipeline. Which of the following is the correct labeling of each component? 

    (True) A) DAG B) Task C) Operator
    A) Task B) DAG C) Operator
    A) Task B) Operator C) DAG
    A) Operator B) Task C) DAG

 

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

 

Which of the following scenarios would be a valid use-case for Airflow? (select all that apply)

    (True) Periodic analysis on sensor data from manufacturing equipment to forecast potential failures and schedule maintenance automatically
    As a dedicated system for processing real-time, high-volume data streams for a stock trading application
    (True) A health care application that schedules email reminders for patients for their appointments
    (True) An AI chatbot that gives tips and solutions based on customer errors and actions

 

The benefits of using a modern data orchestration tool like Airflow is because it offers the ability to...(select all that apply)

    (True) Integrate with hundreds of external systems/software
    (True) Schedule data based on events in addition to time
    Author pipelines as configuration files
    (True) Use a rich feature set with features like built-in observability
    Store, secure and preserve large quantities of data permanently


# 2. Airflow Basics

Airflow core componemts



Fill in the blank: 

The core component of Airflow that serves and updates the user interface is the _____.

    web server

 

Which of the following best describes the role of an executor in Airflow?

    (True) To determine how and where tasks are executed
    To visualize the pipeline runs
    To execute the instructions of tasks
    To store tasks ready to be executed

 

Which of the following best describes the role of the scheduler in Airflow? 

    To store metadata about the state of tasks
    To execute the instructions defined in tasks
    (True) To determine which tasks need to be executed and when
    To define connections to external systems (e.g., Data Warehouses)

 

Which Airflow component is in charge of executing the logic of a DAG's tasks?

    (True) The worker
    The scheduler
    The executor
    The metadata database

___________________________________________________________________________________________________

How does airflow run a DAG?

  

Fill in the blank:

The Airflow scheduler scans for new tasks to run every 5 seconds from the ______.

    meta database

  

After creating your DAG in a Python file, which action do you need to take in order for Airflow to start the process of detecting and running your DAG?

    (True) Put the Python file in the dags directory
    Launch the Airflow web server
    Wait for the scheduler to pick up the tasks defined in the DAG
    Restart Airflow and make sure the DAG is visible on the UI

  

When does the metadata database communicate with the other Airflow components?

    Only when a DAG is starting to run
    Only when a DAG is finished running
    (True) Throughout the entire process of running a DAG



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

  

By default, how long can it take for the Airflow scheduler to detect a new DAG file in the dags directory?

    1 minute
    30 seconds
    5 seconds
    (True) 5 minutes


___________________________________________________________________________________________________



DAG setup



Assume you had a DAG with two tasks: task_one and task_two. The dependency defined in the DAG for these two tasks is: 

task_one >> task_two

Fill in the blank below to correctly describe the dependency relationship: 

task_one is _____ to task_two.

    Answer: "Upstream"

 

Examine the following code:

from airflow import DAG
from airflow.operators.python_operator import PythonOperator

In your own words, what does this code do?
Your response:
Realize imports to identify that file is a DAG

 Correct answer

In which part of a DAG file would you specify how often you want to trigger the DAG?

    In the import statements
    In the DAG's tasks
    (True) In the DAG object definition
    In the DAG's dependencies


___________________________________________________________________________________________________


 

Which of the following Airflow components does the metadata database communicate with? 

    (True) The webserver
    (True) The worker(s)
    The queue
    (True) The scheduler

 

Assume a DAG has 3 tasks: ta, tb, and tc. You want the DAG to execute each task, one after the other, starting with ta, then tb, and finally tc.

Fill in the blank below to correctly define the dependencies of the DAG using either the right (>>) or the left (<<) bitshift operators to reflect the order stated above.

Note: Make sure to include spaces between each task and bitshift operator like so: 
t1 >> t2

    ta >> tb >> tc



Which of the following fills in the following sentence blanks correctly? 

Once a DAG is ready to run, the __________ sends the tasks to the __________. Once a __________ is available, the instructions defined in the task are executed. During the process, the __________ is updated with the DAGs changing state.

    Queue, Metadata Database, Scheduler, Worker
    Scheduler, Worker, Queue, Metadata Database
    Metadata Database, Queue, Worker, Scheduler
    Metadata Database, Queue, Scheduler, Worker
    (True) Scheduler, Queue, Worker, Metadata Database



Assume a DAG has 3 tasks: task_extract, task_transform, and task_load.

Which of the following represents the dependencies in a DAG that needs to meet the following conditions:

task_transform is downstream of task_extract.
task_load is downstream of task_transform.

    (True) task_extract >> task_transform >> task_load
    task_extract << task_load << task_transform
    task_extract >> task_load >> task_transform

# 3. Local Development Environment



Which of the following are benefits of using the Astro CLI for local development? (select all that apply)

    (True) A variety of useful commands for managing an Airflow instance.
    (True) To provide a streamlined experience for installing Airflow with limited pre-requisites.
    (True) Its ability to generate a standard project directory.
    Its ability to dynamically generate new DAGs using AI.



What Astro CLI command will generate a new Airflow project? 

    astro dev init



What is the purpose of the include directory in a new Airflow project generated by the Astro CLI?

    For configuring Airflow instances via environment variables.
    For storing configurations such as connections and variables to prevent loss when recreating the local development environment.
    For the customization of the Airflow instance by adding new operators or modifying the UI.
    (True) For storing files like SQL queries, bash scripts, or Python functions needed in data pipelines to keep them clean and organized.



What Astro CLI command will start running a Airflow project?

    astro dev start



What is the purpose of the airflow_settings.yaml file in a new Airflow project generated by the Astro CLI?

    (True) For storing configurations such as connections and variables to prevent loss when recreating the local development environment.
    For storing Python files corresponding to data pipelines.
    For specifying additional Python packages to install, along with their versions, to extend the functionality of the Airflow environment.
    For configuring Airflow instances via environment variables.


# 4. Airflow User Interface

 

What's the best view to use to optimize your tasks?

    Gantt View
    (True) Landing Times View
    Graph View

 

What's the best view to check the historical states of the DAG Runs and Task Instances for a given DAG?

    (True) Grid View
    Graph View
    DAGs VIew



To identify bottlenecks in your DAG, what's the best view for that?

    Calendar View
    Code View
    (True) Gantt View

 

What's the best view to spot repetitive patterns over many DAG Runs of a DAG?

    (True) Calendar View
    Code View
    Graph View



What does the "Recent Tasks" column on the DAG View show?

    Task's states of current and previous DAG Runs for a given DAG
    (True) Task's states of the current or latest DAG Run for a given DAG

# 5. Airflow DAGs 101



What's the role of the start date?

    (True) Define when the DAG starts being scheduled
    Define the trigger interval
    Avoid running past non-triggered DAG Runs

 

What happens if you don't define a start date?

    Nothing, it's optional
    (True) That raises an error

 

What's the role of tags?

    (True) The allow to better organizing DAGs
    (True) They allow filtering DAGs
    They prevent from running DAGs that do not belong to the current user

 

How can you avoid assigning the dag object to every task you create?

    (True) with DAG(...)
    dag = ...
    (True) @dag(..)
    You can't. You must assign the dag object to every task

 

What happens when two DAGs share the same DAG id?

    The two DAGs appear on the UI
    You get an error
    (True) One DAG randomly shows up on the UI



Does task_a >> task_b >> task_c

is equivalent to

task_c << task_b << task_a?

    (True) Yes
    No

# 6. Airflow Connections 101


 

Can you create two connections with identical ids?

    Yes
    (True) No

 

In Airflow, what is a connection?

    A connection is a way to define the order in which tasks in a DAG should be executed.

    A connection is a type of sensor that waits for a specific condition to be met before proceeding with a task.

    (True) A connection is a way to store and reuse credentials or configuration settings for external systems that are used in Airflow tasks.

 

What is the purpose of defining a connection in Airflow?

    (True) The purpose of defining a connection in Airflow is to avoid hard-coding sensitive information like passwords or API keys into Airflow DAGs, and to allow for easy management and reuse of connection information across multiple DAGs.

    The purpose of defining a connection in Airflow is to store output data from tasks for later analysis.

    The purpose of defining a connection in Airflow is to specify the order in which tasks should be executed within a DAG.

 

What are the different types of connections available in Airflow?

    Airflow only supports one type of connection, which is the SSH connection type.

    (True) Airflow comes with several built-in connection types, including HTTP, MySQL, Postgres, SSH, and more. It also allows you to define custom connection types if needed.

    Airflow supports a very limited set of connection types, including MongoDB, Cassandra, and Redis.


# 7. Airflow Xcom



Select the 4 factors that define the uniqueness of an XCOM

    (True) key
    value
    timestamp
    (True) dag_id
    (True) task_id
    (True) logical_date



Is it possible to push an XCOM without explicitly specifying a key?

    (True) Yes
    No



An XCOM is pushed into..

    The scheduler
    The worker
    The webserver
    (True) The database



With Postgres, can you share 2Gb of data between 2 tasks with an XCOM?

    Yes
    (True) No



How the Scheduler knows which XCOM to choose for a given DAGRun when multiple XCOMs have the same key, dag_id, and task_id?

    It selects one XCOM randomly
    (True) It selects the XCOM based on the logical date
    You can't have multiple XCOMs with the same key, dag_id and task_id


# 8. Airflow Variables

 

With 3 DAGs that fetch data from the same API. Does it make sense to store this API in a variable?

    (True) Yes
    No

 

A variable can be stored in...

    (True) The metadatabase
    (True) A secret backend
    (True) An environment variable
    The metaverse



You create a variable with an environment variable. Does Airflow generate a connection to fetch the value of this variable?

    Yes
    (True) No


Does this code generate a connection to fetch the variable ml_model_parameters every time the DAG is parsed?

    (True) Yes
    No

Does this code generate a connection to fetch the variable ml_report_name every time the DAG is parsed?

    Yes
    (True) No

# 8. Airflow Debug Dags


This DAG doesn’t show up on the UI. Why?

    from airflow.decorators import dag,task
    from pendulum import datetime

    @dag(
        'test_dag',
        start_date = datetime(2023,3,1)
    )
    def test_dag():
        @task
        def test_task():
            return ' Hello World'
        test_task()

    The schedule parameter is missing
    The start_date is in the past
    (True) test_dag() is not called

On manually triggering this DAG you don't see any task execution. Why?

    from airflow.decorators import dag,task
    from pendulum import datetime

    @dag(
        'test_dag',
        start_date = datetime(3030,3,1)
    )
    def test_dag():
        @task
        def test_task():
            return 'Hello World'
        test_task()

    test_dag()

    There is no end_date
    (True) The start_date is in the future
    Because there is only one task and no proper pipeline


How many running DAG runs will you get as soon as you unpause this DAG?

    from airflow.decorators import dag,task
    from pendulum import datetime

    @dag(
        'test_dag',
        start_date = datetime(2023,1,1),
        schedule = '@daily',
        catchup = False
    )
    def test_dag():
        @task
        def my_task():
            return 'Hello World'
        my_task()

    test_dag()

    0
    (True) 1
    16
    32

You just finished writing your DAG and saved the file in the dags folder.

How long will it take to appear on the UI?

    (True) By default it may take up to 5 minutes or more.
    It will be added instantly
    It may take upto 30 seconds.


Is it possible to run tasks that are dependant on different versions of Python in the same DAG?

    (True) Yes
    No

# 9. Airflow Debug Sensors

Manually trigger the DAG first_dag, wait for having 3 tasks running then trigger the DAG second_dag.

What's the task's state of runme in second_dag?

    running
    queued
    (True) scheduled

How many worker slots are used?

(True) 3
2
1

Turn off the schedule of both DAGs and delete the two DAG runs by going to Browse and DAG Runs.

The DAG view should look like that:

    Now,

        Open the file first_dag.py
        Add a new parameter mode='reschedule' in partial()
        Save the file
        Manually trigger first_dag

    What is the status of the three tasks waiting_for_files?

    
    scheduled
    queued
    running
    (True) up_for_reschedule


How many worker slots are running?

    1
    (True) 0
    3


Manually trigger the DAG second_dag.

Does the task runme run?

    (True) Yes
    No

Create a new empty file data_1.csv in the folder include

Go back to the Airflow UI and wait a minute.

What do you see?

    Nothing
    3 tasks are still up_for_reschedule
    (True) 1 sensor has been successfully executed


You can't find the connection type Amazon Web Services. What should you do?

    (True) Install the apache-airflow-providers-amazon
    Install boto3
    Use the http connection type


If the file never arrives in the S3 bucket. When will the S3KeySensor time out?

    In 24 hours
    (True) In 7 days
    Never


Does the Sensor instantly detect the file when it arrives in the bucket?

    Yes
    (True) No, it depends on the poke_interval


A Sensor can be used for (Choose all that apply):

    (True) waiting for files to appear in an S3 bucket
    (True) waiting for a task in another DAG to complete
    (True) waiting for data be present in a SQL table
    (True) waiting for a specified data and time



You have a sensor that waits for a file to arrive in an S3 bucket. Your DAG runs every 10 mins, and it takes 8 mins to complete.

What is the most appropriate timeout duration for the sensor? (in seconds)

    60 * 60 * 24 * 7
    60 * 60
    (True) 60 * 5


What mode doesn't take a worker slot while a Sensor waits?

    poke
    (True) reschedule
    none

What Sensor(s) can be used to apply logic conditions? (Choose all that apply)

    (True) PythonSensor
    (True) @task.sensor
    S3KeySensor


Go on the Airflow doc here and tell me:

What parameter can be useful to check for data to be present in a database without putting too much workload on each poke?

    timeout
    (True) exponential_backoff
    mode


# 9. Airflow Command Line Interface (CLI)


What is the purpose of airflow db init and when might you use it?

    Creates a new user in Airflow
    Generates a report of all DAGs currently in your Airflow environment
    Starts the Airflow web server
    (True) Initializes the Airflow metadata database, typically used when setting up Airflow for the first time


What is the use case for airflow config get-value and how might you use it to troubleshoot issues?

    Lists all of the DAG files that have failed to import
    (True) Retrieves the value of a specific configuration option, useful for verifying that configuration settings are correctly set
    Verifies the validity of the Airflow metadata database schema
    Reserializes a DAG file to ensure that it can be properly loaded by Airflow


You've recently upgraded your Airflow installation, but now your DAGs is not showing up in the UI. Which commands could you use to identify any import/parsing errors that might be preventing the DAG from being loaded?

    (True) airflow dags list-import-errors
    airflow dags show
    (True) airflow dags report
    airflow dags backfill


Why would you use Airflow's backfill functionality?

    To test DAGs before deploying them to a production environment
    To reschedule a DAG to run at a different frequency
    (True) To fill in missing historical data that was not previously captured
    To remove all past DAG runs and start fresh with a new schedule


What does the airflow db check command do?

    Upgrades the Airflow database schema to the latest version
    (True) Checks the connection to the Airflow database
    Removes all data from the Airflow database
    Initializes the Airflow database