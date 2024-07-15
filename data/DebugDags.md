# Debug Dags

- Airflow looks for new dag's every dag_dir_list_interval = 5 minutes by default.

- Updates to dags are reflected after min_file_process_interval = 30 seconds by default.

Other parameters:

 - max_active_runs_per_dag (The maximum number of active DAG runs per DAG). Default → 16.

 - max_active_tasks_per_dag (The maximum number of task instances allowed to run concurrently in each DAG). Default → 16.

 - parallelism (This defines the maximum number of task instances that can run concurrently per scheduler in Airflow, regardless of the worker count). Default → 32.


[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)