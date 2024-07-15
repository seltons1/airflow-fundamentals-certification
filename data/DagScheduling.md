# Dag Scheduling

- What is a DAG run?

    - Default state is queued.
    - By default you can run 16 DAGRuns in the same time.

    Properties:

        - State = Final dag run's state (success or failed).
        - DAG ID = Dag ID of the DAG.
        - Logical Date = Date interval start (date interval start and the execution date).
        - Start Date = Correspoding to the actual timestamp of the start.
        - End Date = Corresponding to when the dag run was completed.
        Duration = Time to complete the dag run.

- How Dag's are scheduled?

        DAG Run 1 (data interval start - 10:00) | (data interval end - 10:10)
        
        DAG Run 2 (data interval start - 10:10) | (data interval end - 10:20)
        
        DAG Run 3 (data interval start - 10:20) | (data interval end - 10:30)

    The dag is trigged after the start_date or last_run + the schedule_interval.

- Dag scheduling parameters

    The schedule_interval

        - Use airflow annotation @daily, @once...
        - Use CRON expression when you want execute you dag in day and time.
        - Use timedelta to schedule each at 3 day ou 3 minutes.

    Schedule in the past

        The catchup parameter:
            Concepts in runs non scheduler Dag run from last run to now (no start date to now)
        
        Backfill your Dags's
            Concepts allows run dag run before start date already existing dag runs.


Resume:

- States of a DAGRun which initially is Queued, and changes to Running as soon as the first task runs. Once all tasks are completed, the final state of the DAGRun is determined by the state of the leaf tasks, which could be Success or Failure.

- The start date and scheduling interval are two important parameters to consider when scheduling a DAG. DAGRuns are created based on these parameters and have a data interval start and end corresponding to the time frame for which the DAG was executed.

- The start date parameter defines the timestamp from which the scheduler will attempt to backfill, and the scheduling interval determines how often a DAG runs.

- The catchup mechanism in Airflow allows running all non-triggered DAGRuns between the start date and the last time the DAG was triggered. The backfilling mechanism allows running historical DAGRuns or rerun already existing DAGRuns.

- We also explored the Airflow CLI commands to backfill our DAG for any data intervals, regardless of the start date of our data pipeline.

- Users can define the scheduling interval using CRON expressions or timedelta object, and can use a timetable to schedule a DAG more precisely.

- It is important to set the start date parameter properly to avoid confusion with Airflow, and use a static date.

[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)