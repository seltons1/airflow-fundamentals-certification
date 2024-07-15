# Connections

- What is a connection?

    - An Airflow Connection stores credentials to interact with external systems (S3, Snowflake, etc).
        
    - A Connection is a set of parameters such as login, password, host and some specific fields that depend on the Connection type.
    
    - A Connection type corresponds to the external system you want to interact with: Snowflake, Postgres, MySQL etc.
    
    - If the Connection type isn't available, you must install the corresponding Airflow provider.
    
    - A Connection must have a unique identifier.
    
    - To use a Connection in an Operator, refer to it using the Connection identifier.
        