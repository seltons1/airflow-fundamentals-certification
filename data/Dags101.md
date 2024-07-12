# DAG's 101

- What's a DAG?

In Airflow, a directed acyclic graph (DAG) is a data pipeline defined in Python code. Each DAG represents a collection of tasks you want to run and is organized to show relationships between tasks in the Airflow UI. The mathematical properties of DAGs make them useful for building data pipelines:

    Directed: If multiple tasks exist, each must have at least one defined upstream or downstream task.

    Acyclic: Tasks cannot have a dependency on themselves. This avoids infinite loops.
    
    Graph: All tasks can be visualized in a graph structure, with relationships between tasks defined by nodes and vertices.

Aside from these requirements, DAGs in Airflow can be defined however you need! They can have a single task or thousands of tasks arranged in any number of ways.

- Defining your DAG!

With the traditional paradigm, we've created the following DAG:

    from airflow import DAG
    from datetime import datetime

    with DAG('my_dag', start_date=datetime(2023, 1 , 1),
            description='A simple tutorial DAG', tags=['data_science'],
            schedule='@daily', catchup=False):


- Define your first task

With the traditional paradigm, you must:

    Import the Operator
    Call the Operator 
    Define the task_id and other parameters


- The default arguments

As you know, you can apply different arguments to your tasks. For example, the number of retries before failing, the execution timeout, if you want to receive an email on failure, etc.

By default, the number of retries for a task before failing is set to 0.

A DAG object can take an option default_args parameter that allows defining common arguments to all tasks in your DAG.

Let me show you an example:

    default_args = {
        'retries': 3,
    }

    with DAG('my_dag', start_date=datetime(2023, 1 , 1), default_args=default_args,
            description='A simple tutorial DAG', tags=['data_science'],
            schedule='@daily', catchup=False):
        
        task_a = PythonOperator(task_id='task_a', python_callable=print_a)
        task_b = PythonOperator(task_id='task_b', python_callable=print_b)
        task_c = PythonOperator(task_id='task_c', python_callable=print_c)
        task_d = PythonOperator(task_id='task_d', python_callable=print_d)
        task_e = PythonOperator(task_id='task_e', python_callable=print_e)

        chain(task_a, [task_b, task_c], [task_d, task_e])



[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)