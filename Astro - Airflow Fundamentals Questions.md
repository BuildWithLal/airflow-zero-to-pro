## Airflow Use Cases

**1. When is Airflow the best solution for a workflow?**  
a) Real-time data processing  
b) Orchestrating complex workflows with dependencies  
c) Storing large datasets  
d) Serving APIs directly  
Answer: b  

**2. Which of the following is NOT a use case for Airflow?**  
a) Scheduling ETL pipelines  
b) Automating CI/CD pipelines  
c) Real-time stream processing  
d) Orchestrating machine learning workflows  
Answer: c  

---

## Airflow Concepts

**3. What does the Airflow Scheduler parse to identify new DAGs?**  
a) logs_folder  
b) dags_folder  
c) plugins_folder  
d) include_folder  
Answer: b  

**4. What is a DAG in Airflow?**  
a) A group of related tasks without dependencies  
b) A workflow representation with dependencies  
c) A database for storing logs  
d) A configuration file for Airflow connections  
Answer: b  

**5. What is the purpose of XComs in Airflow?**  
a) To define dependencies between tasks  
b) To transfer data between tasks  
c) To monitor DAG runs  
d) To schedule tasks  
Answer: b  

**6. What is the default time zone for an Airflow instance?**  
a) UTC  
b) PST  
c) Local system time  
d) EST  
Answer: a  

**7. What is the primary role of an Airflow worker?**  
a) Scheduling DAGs  
b) Parsing DAG files  
c) Executing tasks  
d) Monitoring system logs  
Answer: c  

**8. Which of the following is a valid Airflow operator?**  
a) DataOperator  
b) DAGOperator  
c) PythonOperator  
d) ScriptOperator  
Answer: c  

---

## Dependencies

**9. Where are task dependencies defined in Airflow?**  
a) Inside the Airflow configuration file  
b) Directly in the DAG file  
c) In the Airflow UI  
d) In the airflow.cfg file  
Answer: b  

**10. Which of the following symbols is used to set upstream task dependencies in Airflow?**  
a) =  
b) >>  
c) <<  
d) Both b and c  
Answer: d  

---

## Airflow CLI

**11. Which Airflow CLI command initializes the metadata database?**  
a) airflow dags init  
b) airflow db init  
c) airflow initdb  
d) airflow db upgrade  
Answer: b  

**12. Which CLI command can you use to test a specific task in a DAG?**  
a) airflow tasks execute  
b) airflow tasks run  
c) airflow tasks test  
d) airflow dags test  
Answer: c  

---

## Airflow UI

**13. Which Airflow UI view is best for identifying task dependencies?**  
a) Grid view  
b) Graph view  
c) Tree view  
d) Gantt view  
Answer: b  

**14. What does the “Last Run” column in the Airflow UI indicate?**  
a) The last time a task succeeded  
b) The last time a DAG run started  
c) The most recent log update for a task  
d) The last time the Airflow Scheduler was restarted  
Answer: b  

**15. Which UI view provides information about task duration over time?**  
a) Graph view  
b) Grid view  
c) Gantt view  
d) Tree view  
Answer: c  

---

## DAG Scheduling

**16. What is the purpose of the schedule_interval parameter in a DAG?**  
a) To define the order of tasks in the DAG  
b) To set the time intervals for DAG runs  
c) To determine task dependencies  
d) To specify the timezone for the DAG  
Answer: b  

**17. Which value for schedule_interval will run a DAG every day at 2 PM?**  
a) @daily  
b) @hourly  
c) 0 14 * * *  
d) 0 2 * * *  
Answer: c  

**18. What happens if catchup is set to False in a DAG?**  
a) The DAG will backfill all past runs automatically.  
b) The DAG will only run future tasks and skip missed runs.  
c) The DAG will only execute on demand.  
d) The DAG will fail on missed runs.  
Answer: b  

---

## Debugging

**19. Which Airflow CLI command is used to clear a failed task?**  
a) airflow tasks clear  
b) airflow tasks retry  
c) airflow tasks reset  
d) airflow tasks re-run  
Answer: a  

**20. What might cause a DAG to fail during parsing?**  
a) Circular dependencies in the DAG definition  
b) Using unsupported operators  
c) Missing dag_id in the DAG definition  
d) All of the above  
Answer: d  

---

## XComs

**21. Which of the following methods is used to push data to an XCom?**  
a) task.push_xcom()  
b) task.xcom_push()  
c) task.data_push()  
d) xcom.push()  
Answer: b  

**22. What is a limitation of XComs in Airflow?**  
a) They cannot store JSON data.  
b) They are limited to transferring small amounts of data.  
c) They cannot transfer data between DAGs.  
d) They can only be used with Python operators.  
Answer: b  

---

## Operators

**23. What is the purpose of the PythonOperator in Airflow?**  
a) To execute SQL queries  
b) To run arbitrary Python functions  
c) To move data between databases  
d) To monitor file availability  
Answer: b  

**24. What does a Sensor operator do in Airflow?**  
a) Executes Python code  
b) Waits for a specific condition to be met  
c) Transfers data between systems  
d) Monitors task status in a DAG  
Answer: b  
