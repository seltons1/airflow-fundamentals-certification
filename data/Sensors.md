# Sensors

- Sensors wait for an event/condition to be met to complete
By default, a Sensor times out after 7 days. You should define a better value with the timeout parameter.

- A sensor checks an event/condition at every poke_interval (60 seconds by default).

- While a sensor waits, it continuously takes a work slot.

- If you have many sensors or expect them to take time before complete, use the reschedule mode.

- With the reschedule mode, while a sensor is waiting, its status will be up_for_reschedule.

- You can create a sensor with @task.sensor .

When using sensors, keep the following in mind to avoid potential performance issues:

- Always define a meaningful timeout parameter for your sensor. The default for this parameter is seven days, which is a long time for your sensor to be running. When you implement a sensor, consider your use case and how long you expect the sensor to wait and then define the sensor's timeout accurately.

- Whenever possible and especially for long-running sensors, use the reschedule mode so your sensor is not constantly occupying a worker slot. This helps avoid deadlocks in Airflow where sensors take all of the available worker slots.

- If your poke_interval is very short (less than about 5 minutes), use the poke mode. Using reschedule mode in this case can overload your scheduler.

- Define a meaningful poke_interval based on your use case. There is no need for a task to check a condition every 60 seconds (the default) if you know the total amount of wait time will be 30 minutes.


[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)