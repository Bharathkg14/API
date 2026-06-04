Need admin to create CORTEX_POC DB (request sent)


Isolation. We’re running AI functions that generate new tables, views, and ML models. Doing this in a dedicated CORTEX_POC database means:

Zero risk to production — no accidental writes to COMM_DEV.GOLD
Easy cleanup — drop one database when POC ends, no orphan objects
Clear ownership — my role owns it, no permission conflicts with shared schemas


Could you please:

Create a new database called CORTEX_POC
Grant full ownership of that database to my role COMM_ETL_SVC_RL_DEV
Ensure my role has usage on warehouse COMM_US_WH_DEV
Confirm that my role has Cortex access (SNOWFLAKE.CORTEX_USER)
This will allow me to:

Create schemas, tables, and views
Create stored procedures
Train anomaly detection models
Use Cortex AI functions
