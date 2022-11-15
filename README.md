# Event and Log Data Modeling with CassandraQL (AP-NoSQL)

## Background

	A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. 
	The analysis team is particularly interested in understanding what songs users are listening to. 
	Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

## Objective

    - Event and Log data tables Designed for data analysis. 
    - Queries optimization on with a Cassandra Database.
    - ETL pipeline and partial table or data for data analysis.
    - Evaluated and test queries data modeling with Sparkify's expected results.

### Data Fields and prerequisites for each 3 tables in this project
## Key Point 1 Query 1 Table !

    Frist table, For get artist name, song title and length

	prerequisites = PRIMARY KEY (sessionid, iteminsession) :
        1. artist
        2. song_title
        3. length
        4. level
        5. sessionid
        6. iteminsession

   Second table, For get artist name, song title, user's firstname and user's lastname

	prerequisites = PRIMARY KEY((userid, sessionid), iteminsession) :
    users table:
        1. artist
        2. song_title
        3. firstname
        4. lastname
        5. userid
        6. sessionid
        7. iteminsession

   Third table, For get user's firstname and user's lastname

	prerequisites = PRIMARY KEY(song_title, firstname, lastname)) :
    songs table:
        1. song_id
        2. title
        3. artist_id
        4. year
        5. duration

## Project files

- `event_datafile_new.csv` - Dataset for processing and testing.
- `Project_1B_ Project_Template.ipynb` - implementation file such as ETL processing and queries results.

    
## How to run ?
    0. Open Project_1B_ Project_Template.ipynb and follow steps by steps
    1. Done !! 
    
## My git : https://gist.github.com/MosesOhYes
## My Repository : https://github.com/MosesOhYes/Data-Modeling-with-Apache-CassandraDB.git
