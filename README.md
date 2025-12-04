1. Go to https://app.snowflake.com/

login/logon

Create Warehouse

create Database

create role

2. open vscode : 

pull all python scripts.

3. create .env

SNOWFLAKE_USER=

SNOWFLAKE_PASSWORD=

SNOWFLAKE_ROLE=

SNOWFLAKE_ACCOUNT=

SNOWFLAKE_WAREHOUSE=

SNOWFLAKE_DATABASE=

SNOWFLAKE_SCHEMA=

4. run

  1.create_tables_schemas.py

  2.create_stored_precedure.py​

  3.load_data_to_snowflake.py​

5. back to snowflake

run below procedures step by step

CALL STAGE.SP_LOAD_STG_REPOSITORIES();

CALL LINKMAP.SP_LOAD_HUB_REPO_CONTRIBUTORS();

CALL LINKMAP.SP_LOAD_HUB_REPO_COMMITS();

CALL LINKMAP.SP_LOAD_HUB_REPO_ISSUES();

CALL LINKMAP.SP_LOAD_HUB_REPO_RELEASES();

CALL ENRICH.SP_LOAD_REPO_ENTRYLINE();

CALL CURATE.SP_LOAD_RISK_ANALYSIS_DATA_PRODUCT();

6. Back to VScode

run risk_analysis.py (follow readme_risk_analysis for report generation)

7. run create_monitoring_view.py

To check the view, back to snowflake (follow readme_monitoring.md)


