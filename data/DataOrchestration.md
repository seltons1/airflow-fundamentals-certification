# Data Orchestration

Able to build data pipeline that coordinate diferent tools to answer a specific business need.

Data orchestration is the coordination and automation of data flow across various tools ans systems to deliver quality data products and analytics.

# Journey to Modern Data Orchestration

    # PRE-UNIT ERA
    
        - Defined by 
        
            - Manual batch-processing and scheduling.
        
            - The foundation of the idea and need of data orchestration and workflow management starting to form.

        - Limitations

            - The entire process was manual and error-prome it depended on humans to catch erros and fix them.

            - Lack of standartization of data formats, protocols and processing techniques.
_________________________
    #EARLY COMPUTING (Such as CRON or WTS)
        
        - Defined by

            - Basic time-based scheduling tools.

            - A subsequent rise of proprietary scheduling do workloads management tools.

            - Dedicated ETL tooling.

        - Limitations

            - Proprietary software was expensive, close-source and resource intensive.

            - Schedulers like CRON and WTS lacked features for more complex workloads and general maintainbility.

_________________________
    #DATA & OPEN-SOURCE RENAISSANCE (Such as Luigi, Ozie and Azkaban)
        
        - Defined by

            - Increase in data complexity and size.
            
            - Increase in complexity of scheduling and ETL workloads.

            - Rise of open-source workflow management projects. 

        - Limitations

            - Some tools were limited to working only within the hadoop ecosystem.

            - Some tools used XML and config files to define workloads.

            - Limited dynamism, scalability and extensibility.

_________________________
    #MODERNS DATA ORCHESTRATION
        
        - Defined by

            - Rise of pipelines-as-code in python.

            - The ability to integrate with hundreds of external systems.

            - Time and event-based scheduling.

            - Feature rich software with built-in observability and centralized UI.



[Back to Main](https://github.com/seltons1/airflow-fundamentals-certification/blob/main/README.md)