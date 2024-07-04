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



[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)