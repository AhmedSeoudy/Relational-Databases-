- Summary:

This project models user activity data for a music streaming app called Sparkify to optimize queries for understanding what songs users are listening to by creating a Postgres relational database and ETL pipeline to build up Fact and Dimension tables and insert data into new tables

- Run the Python scripts:
    1. Open Terminal
    2. Run the command 'python create_tables.py'
    3. Run the command 'python etl.py'
    
- Project Structure:

# Dataset
1. log_data
2. song_data
# notebook for developing and testing ETL
1. etl.ipynb     # developing ETL builder
2. test.ipynb    # testing ETL builder
# source code
1. etl.py               # ETL builder
2. sql_queries.py       # ETL query helper functions
3. create_tables.py     # database/table creation script    

etl.py --> ETL pipeline builder

process_data
Iterating dataset to apply process_song_file and process_log_file functions
process_song_file
Process song dataset to insert record into songs and artists dimension table
process_log_file
Process log file to insert record into time and users dimensio table and songplays fact table

create_tables.py --> Creating Fact and Dimension table schema

create_database
drop_tables
create_tables
sql_queries.py

Helper SQL query statements for etl.py and create_tables.py

*_table_drop
*_table_create
*_table_insert
song_select


  
    
    