Links:
Primary Dataset: 
https://www.kaggle.com/datasets/rodolfofigueroa/spotify-12m-songs

# id,name,album,album_id,artists,artist_ids,track_number,disc_number,explicit,danceability,energy,key,loudness,mode,speechiness,acousticness,instrumentalness,liveness,valence,tempo,duration_ms,time_signature,year,release_date

1. Primary Dataset: tracks_features.csv: The Historical "Loudness War"

2 Questions: Between 1960 and 2015 (pre-TikTok era), how did the average loudness and duration_ms of songs change annually?
loudness vs year
duration_ms vs year




2. Supplementary Datasets:
https://github.com/Sveta151/TikTok_impact_on_the_top_charts

Spotify Top Charts vs TikTok Songs (2019-2022)
How many popular songs on TikTok appear on Spotify top charts per year...


# track_name,artist_name,artist_pop,album,track_pop,danceability,energy,loudness,mode,key,speechiness,acousticness,instrumentalness,liveness,valence,tempo,time_signature,duration_ms
tiktok_songs_YEAR.csv 

What audio features (danceability, energy, loudness, acousticness, etc.) are associated with TikTok virality?


# uri,artist_names,track_name,peak_rank,weeks_on_chart,danceability,energy,key,loudness,mode,speechiness,acousticness,instrumentalness,liveness,tempo,time_signature,duration_ms
spotify_top_charts_YEAR.csv

COMPARING BOTH SUPPLEMENTARY DATASETS
Do songs trending on TikTok stay longer on Spotify top charts than non-TikTok songs?
TikTok: track_name, artist_name
Spotify: track_name, artist_name, Weeks on Chart
(compare)


COMPARING TIKTOK_SONGS_YEAR.CSV TO PRIMARY DATASET
What is the average audio features of tiktok viral songs compared to songs before tiktok (median/average of everything (pre 2016) vs median/average of tiktok (only viral tiktok songs))







QUESTIONS:
How has the average loudness and duration_ms of songs change annually?
How many popular songs on TikTok appear on Spotify top charts per year?
Do songs trending on TikTok stay longer on Spotify top charts than non-TikTok songs?
Has danceability and energy increased after TikTok?
How has track features changed over time? 




Attributes Needed:
Primary: name,artists,danceability,energy,key,loudness,tempo,duration_ms,time_signature,year
TIKTOK Supplementary: track_name,artist_name,danceability,energy,loudness,key,tempo,time_signature,duration_ms
SPOTIFY Supplementary: artist_names,track_name,danceability,energy,key,loudness,tempo,time_signature,duration_ms





<-Plan->
Mar 16 (3 hours)	
Identify problem/project idea, brainstorm datasets, and draft research questions

Mar 17 (3–4 hrs)	
Find & download datasets, create virtual environment, load datasets into dataframes	

Mar 18 (4 hrs)	
Filter datasets to keep only relevant columns, merge datasets for relationships, Design ERD, create database schema	

Mar 19 (4 hrs)	
Load schema into SQL, update dataframes to match schema, Load dataframes into database, verify data integrity

Mar 20 (3 hrs)	
Sketch visualizations/dashboards, plan structure, Create Docker setup (docker-compose.yaml), Set up Airflow folder	

Mar 23 (4 hrs)	Set up Airflow folder, Refactor ETL into music_etl_dag.py, test Airflow DAGs, Ensure database loads correctly

Mar 24 (6 hrs)	Finish Airflow DAGs, Made Visualizations, Created diagram of dataflow

Mar 25 (3 hrs)	Finished Visualizations, wrote report + started on presentation

Mar 26 (4 hrs)	Finished presentation, Practiced presenting, Webpage improvements 

Mar 27 	        Present



APA CITATIONS:
Figueroa, R. (n.d.). Spotify 12M+ songs [Data set]. Kaggle. https://www.kaggle.com/datasets/rodolfofigueroa/spotify-12m-songs
Sveta151. (2022). TikTok impact on the top charts [Source code]. GitHub. https://github.com/Sveta151/TikTok_impact_on_the_top_charts


Other sources:
https://plotly.com/python/subplots/
https://plotly.com/python/plotly-express/
https://dash.plotly.com/tutorial