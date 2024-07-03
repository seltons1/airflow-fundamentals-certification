# Airflow Core Components

    WEBSERVER (Flask Web Server)
        
        Enable users to monitor task execution, view status of dags, access the logs (serving and updating the UI).
    
    METADATA DATABASE

        Contains all the metadata to airflow instance such as task instances, DAG status, users. Comunicates with webserver, scheduler and executor.

    SCHEDULER (Monitoring and Scheduling tasks)

        Is a critical component of the airflow , is responsible for determining which task to execute and when.

    EXECUTOR (Part of Scheduler)

        Defines how and which system to execute yout tasks.

    QUEUE

        Make sure that the tasks run in the correct order as specified in your data pipeline.

    WORKERS

        The workers take the tasks from the queue in order to execute then.

    TRIGGERER
        Is responsible for managing a specific kind of operator called the defenable operator.

    
# How does Airflow Run a DAG?

What's happening when do you create a new pipline and add in /dags folder?

    1. The scheduler verify dags directory for new files, every 5 minutes by default.

    2. After that the file is processed into the metadata database.

    3. Scheduler scans every 5 seconds dags that are ready to run.

    4. If dags ready, its tasks are put into the executors queue.

    5. When worker is avaliable, it will take a task to execute from the queue.

    6. The metadata database will be updated when a dag is running.

    7. Finally webserver can access status of tasks and associated errors.

# DAG Setup

    Dag is divided in 4 parts:

        - Import Statments

        - Dag Object

        - Task Operators

        Task Dependencies (using bitshift operator ">>" or "<<")


[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)