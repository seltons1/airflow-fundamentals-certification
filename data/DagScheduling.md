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

