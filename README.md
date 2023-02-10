

# Spark_&_Data_Lakes

# Table of Content

## Schema for Song Play Analysis

##### Fact Table

songplays - records in log data associated with song plays i.e. records with page NextSong
songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent

##### Dimension Tables

users - users in the app
user_id, first_name, last_name, gender, level
songs - songs in music database
song_id, title, artist_id, year, duration
artists - artists in music database
artist_id, name, location, lattitude, longitude
time - timestamps of records in songplays broken down into specific units
start_time, hour, day, week, month, year, weekday

<img width="1283" alt="Screen Shot 2023-02-10 at 12 24 50 PM" src="https://user-images.githubusercontent.com/103359089/217999352-9c5d2f94-3f42-43ac-8de6-991206cd8425.png">


##### Project Datasets

Song data: s3://udacity-dend/song_data
Log data: s3://udacity-dend/log_data



##### Project Template

etl.py reads data from S3, processes that data using Spark, and writes them back to S3
dl.cfgcontains  AWS credentials
README.md provides discussion on the over all project


# Executive Summary

A music streaming startup, Sparkify, has grown their user base and song database even more and want to move their data warehouse to a data lake. Their data resides in S3, in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

They request a  data engineer to building an ETL pipeline that extracts their data from S3, processes them using Spark, and loads the data back into S3 as a set of dimensional tables.


# Executing

Fill in the access key Id and the secret access key to connect and have access to S3 bucket.

[S3]
AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

# To initiate the ETL pipeline

Run python etl.py on the terminal
if successful the preview will be displayed

