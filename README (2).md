Purpose of Database
--------------------------

The aim of the dashboard is the analyze the data of Sparkify that it has been collecting on songs and user activity on their music streaming app. One of the most significant aims of the project is to understand what songs the users are listening to.

We want to create a database schema and ETL pipeline to pull the data from the JSON files in which the data is contained to optimise queries on song play analysis. 


How to Run Python Scripts
--------------------------

Python scripts can be run through the terminal using the prefix python3. For example, open Terminal and type python3 create_tables.py


Description of Files
--------------------------

create_tables.py - Python file to trigger the creation of the database. This script also imports table creation and table deletion functions from the sql_queries.py file.

etl.ipynb - an interactive Python notebook used for testing the etl process

etl.py - Python file to trigger the ETL process for the data from the JSON song and logs files.

sql_queries.py - Python file containing the query strings for table creation and deletion, record insertion and specific select test queries.

test.ipynb - an interactive Python notebook used for running sanity, naming, primary key, constraint and upsertion tests.


Schema Design
--------------------------

Data is organised in a star schema structure. This is through 4 dimension tables (users, artists, time and songs) and 1 fact table (songplays). This design was chosen to make it easy for business users to query the table through a denormalized database design.