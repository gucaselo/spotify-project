# Spotify Project
This project is an overview of the Spotify Weekly Top 200 Charts and how music streaming was affected during Covid-19

## Table of Contents
* [General Info](#general-info)
* [Technologies](#technologies)
* [Scope of Work](#scope-of-work)
* [Data Overview](#data-overview)
* [References](#references)
* [Spotify Defined Elements](#defined-elements)


### General info
Objective: We set out to identify any change in trends within Spotify Top 200 music streaming charts from 2019 to 2020 due to world events such as, the Covid-19 pandemic.

Hypothesis: Music streaming volume is likely to increase and patterns in users’ music selection will shift to more tracks that are lower in energy, less dancible, and overall have a more sorrowful mood.

### Technologies
- Python
- Pandas
- Matplotlib
- Seaborn
- Spotify API
- Squarify

### Scope of Work
- Pull and merge weekly CSVs from Spotify.
- Created a spotify client to be utilized to make API calls to retrieve additional data including Spotify audio features.
- Perform comparative analysis between 2019 and 2020 datasets.
- Analyze Genres.
- Perform Audio Analysis and determine any correlation between Spotify audio features.
- Compare any changes in audio features between 3 countries that drastically different pandemic response measures.
- Indentify any trends for an individual track within the Top 200 Chart.

### Data Overview
Our data shows a 6.5% (1.9 billion) decrease in streams in 2020.  Albeit having fewer streams 2020 showed an increase in total artists (+24), tracks (+111), and 70 total genres (+212%)  in the Top 200.

Next we show the differences between Spotify's elements and features.  A further look is taken into Danceabitlity and Energy because of their positive correlation.

Radar, Bar, and Desity plots are used to show the Music Moods and distribution in the first 6 months of 2020 for the United States, Italy, and Sweden.  These three countries were picked based on the decisions on how to handle the Covid 19 pandemic.  

We chose to take a deep dive into the artist The Weeknd and his single 'Blinding Lights' about how other factors can affect streams.  The charts follow the release dates and performances throughout the year.

<img src="output_plots/Density Plot of Sweden, Italy and USA in March (Valence).png"/>


### Output
All created CSV files are saved in output_Data and all visuals are saved in output_plots

#### References
###### https://developer.spotify.com/documentation/web-api/
###### https://spotifycharts.com/
###### https://everynoise.com/

#### Defined Elements
###### Danceability: Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat -strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.

###### Energy: Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.

###### Speechiness: Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.

###### Valence: A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).

###### Acousticness: A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.

###### Instrumentalness: Predicts whether a track contains no vocals. “Ooh” and “aah” sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly “vocal”. The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0

###### Liveness: Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.

