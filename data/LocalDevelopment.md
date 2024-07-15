# Local Development Environment

There are two primary ways to install Airflow on a local machine: Python Package Index or Containerization Solutions (e.g., Docker, Podman)

        The Python Package Index

            - This method is great for anyone who is comfortable with Python and Python environments or may only have access to it in their local environment 

            - This method does require quite a bit of manual setup to get Airflow working on a local machine

        Containerization Solutions
            
            - This method is great for anyone familiar or already using a containerization solution
            
            - This method may still require a bit of customization to the container if the Airflow installation needs to be fine-tuned

    The Astro CLI is an open-source command line interface (CLI) that makes setting up, running, and managing Airflow a breeze. It comes built-in with a handful of features to make it easier to get started quicker. 
    
    Alternatives to the Astro CLI include using the Airflow CLI, which is built-in to Airflow, or another open-source project called AirflowCTL
    Astro CLI can be installed on Mac, Windows, and Linux machines by following the instructions listed in the documentation.

# Set up and Run an Airflow Project

    To set up a new Airflow project with the Astro CLI, make a new folder, and then use the command astro dev init to generate a new project.

    The Astro CLI will generate a project with a standard project directory. This includes:
        
        - The dags directory: Contains Python files corresponding to data pipelines, including examples such as example_dag_advanced and example_dag_basic.
        
        - The include directory: Used for storing files like SQL queries, bash scripts, or Python functions needed in data pipelines to keep them clean and organized.
        
        - The plugins directory: Allows for the customization of the Airflow instance by adding new operators or modifying the UI.
        
        - The tests directory: Contains files for running tests on data pipelines, utilizing tools like the pytest library.
        
        - The .dockerignore file: Describes files and folders to exclude from the Docker image during the build.
        
        - The .env file: Used for configuring Airflow instances via environment variables.
        
        - The .gitignore file: Specifies files and folders to ignore when pushing the project to a git repository, useful for excluding sensitive information like credentials.
        
        - The airflow_settings.yaml file: Stores configurations such as connections and variables to prevent loss when recreating the local development environment.
        
        - The Dockerfile: Used for building the Docker image to run Airflow, with specifications for the Astro runtime Docker image and the corresponding Airflow version.
        
        - The packages.txt file: Lists additional operating system packages to install in the Airflow environment.
        
        - The README file: Provides instructions and information about the project.
        
        - The requirements.txt file: Specifies additional Python packages to install, along with their versions, to extend the functionality of the Airflow environment.

The Astro CLI can be used to run an Airflow project. To start an Airflow project with the Astro CLI, use the command astro dev start. To restart the project, use astro dev restart, and to stop the project, use the command astro dev stop.

To get Airflow to work with VSCode and provide benefits like correct syntax highlighting and autocompletion, the VSCode instance must be run inside of the docker container using the Dev Containers extension.


- DAGs and Task Instances

Use tags to categorize or organize your data pipelines.
"Runs" shows the status of the past and most recent DAG runs. Whereas "Recent Tasks" shows only the status of the task instances for the active or most recent DAG runs.
"Last run" is the data interval start of the last DAG run
"Next run" is the data interval start of the next DAG run
The "Delete DAG" button doesn't delete the DAG file, only the metadata related to the DAG.
Don't forget to remove any applied filters or you may wonder why a DAG doesn't show up on the UI. It's an easy mistake.

- Monitor Dag and Task Instance

The mean run duration + buffer is the correct value for defining a timeout for your DAG. 
The grid view shows previous and current DAG runs with their task instances and states.
The top bars are the DAG runs. The squares are the task instances.
The longer a top bar is, the longer it took to complete that specific DAG run.
You get a DAG runs summary when you land on the Grid view. Mean run duration helps define the DAG's timeout.
Share information with the rest of your team using notes. That applies to DAG runs and task instances.
Clear restarts the selected DAG run or task instance.
When you want to clear a task instance, not including Downstream means downstream tasks to the selected task won't be rerun.
Use shortcuts if you...

- Check Task Dependencies

The Graph view is perfect for checking dependencies between tasks of a DAG.
A rectangle is a task with information such as the operator and the state.
Use the mini-map for navigating a large data pipeline with many tasks.

- Detecting Trends and Patterns

The Calendar view overviews your entire DAG's history over months or even years.
The Calendar view is perfect to spot breaking patterns or trends.
A square is a day, and the color of that square depends on the ratio between successful and failed DAG runs.
Squares with dots indicate that DAG runs are planned for these days.

- Optimize Your Tasks

Landing times are calculated from the task scheduled time to the time the task finishes (end_time - scheduled_time)
Landing times correspond to the actual execution time of your tasks.
Task durations (the other view) show the total task durations (scheduled time included)
This view is perfect for evaluating the effectiveness of your changes.

- Find Bottlenecks in Your DAG Runs

The Gantt chart is perfect for identifying task bottlenecks and overlaps.
A rectangle is a task. The longer the rectangle, the longer it took to complete the task.
A rectangle is divided into two parts. The first part (grey) is the queued time. The second is the execution time.
The queued time corresponds to the time spent waiting for a worker to pick your task. A worker executes tasks.
Two rectangles side by side mean tasks have been executed in parallel and this is an overlap.

- Check DAG Updates

The Code view shows the DAG code parsed by the Scheduler.
The Code view is perfect for checking whether or not DAG updates have been picked up.
Look at the Parsed at date instead of searching for your modification in the code.
You can't edit DAG code in the Code view.

- Debugging Tasks

A DAG run fails when a task fails in it.
The first step to debug a task instance is to look into the logs.
You get different logs for each retry (attempt) to the same task.
Pause the DAG before fixing the error. Otherwise, your DAG runs will continue to fail.
Retry multiple DAG Runs and Task instances at once using Browse.

- Browse DAG Runs and Task Instances

From "Browse", you can have lists of DAG runs, Task instances, Jobs, and more.
Use "Browse" to simultaneously take actions on multiple DAG runs or Task instances.
You can search on specific objects by mixing different filters.
You can rerun a set of task instances of DAG runs by filtering on the start and end dates. Then select Clear the state.
"Browse" provides further details on your Task instances or DAG runs, such as, run type, start date, duration, etc.


[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)