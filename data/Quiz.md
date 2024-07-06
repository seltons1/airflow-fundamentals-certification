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

        