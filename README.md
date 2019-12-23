# Project 1: Data Modeling with Postgres

The purpose of this project is to understand which songs are the most listened to by the user. To do this, you have to design a database in Postgres with the queries configured to make the intake in this database.

### Justification for the design of the database and ETL pipeline scheme.

We have 2 datasets, songs and logs in format, each consisting of several json files.

1. We will create the connection to the bbdd, the bbdd and the tables, **"songsplays"** (fact table) and **"users", "songs", "artist" and "time"** (tables of dimensions). To do this we implement the file **"sql_queries.py"**, creating the CREATE and DROP statements that will be responsible for creating the tables if they do not exist and delete them.

2. We will create the datasets themselves with the fields indicated in the exercise and insert the corresponding records in the tables created above. To do this, we will use the **"etl.ipynb"** file where we will carry out the tests before implementing the **"etl.py"** file that will be responsible for loading the data in the databases of the database.

Finally and once the data is ingested in the different tables we can already carry out the queries indicated in the exercise.