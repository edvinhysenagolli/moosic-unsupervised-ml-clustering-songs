# Moosic: Unsupervised Music Playlist Clustering Project
Moosic is a growing start-up that specializes in creating personalized music playlists curated by music experts and enthusiasts. As their user base expands, the company is faced with the challenge of manually curating new playlists to match user preferences and moods. To address this, they've brought in data science expertise to introduce a level of automation to their playlist creation process.

## Project Overview
The primary objective of this project is to utilize data science techniques to automate the process of creating music playlists based on audio features. Moosic has access to a dataset obtained from the Spotify API, which contains audio features such as tempo, energy, danceability, and more for a collection of songs. The goal is to apply a basic clustering algorithm, specifically the K-Means algorithm, to group songs with similar audio features into clusters. These clusters will then serve as the foundation for creating playlists that capture distinct "moods" or "styles."

## Business Context
Moosic aims to balance human-curated playlists with data-driven playlist creation. While some team members are skeptical about whether audio features can capture the emotional nuances of songs, others believe that data science can uncover unique connections between songs that might be missed by human curators. This project's initial phase focuses on creating a prototype that can assist in playlist creation. The key assessments include:

- Identifying Similar Songs: Can Spotify's audio features effectively identify songs that are similar based on human-perceivable criteria? Can these features capture musical traits that align with common human understanding of song moods or styles?

- Effectiveness of K-Means: Is K-Means a suitable algorithm for creating playlists? Should alternative clustering methods be explored for playlist generation?

## Data and Features
The dataset for this project contains various audio features provided by Spotify's API. These features include:

`acousticness`: Confidence measure of whether the track is acoustic.

`danceability`: Suitability of a track for dancing based on tempo, rhythm, etc.

`duration_ms`: Duration of the track in milliseconds.

`energy`: Measure of intensity and activity in a track.

`instrumentalness`: Predicts whether a track contains vocals.

`key`: The key in which the track is.

`liveness`: Detects the presence of an audience in the recording.

`loudness`: Overall loudness of a track in decibels.

`mode`: Modality (major or minor) of a track.

`speechiness`: Detects the presence of spoken words in a track.

`tempo`: Estimated tempo of a track in beats per minute.

`time_signature`: Estimated overall time signature of a track.

`valence`: Measure of musical positiveness conveyed by a track.

## Data Preparation
The initial phase of the project involves data preparation:

### Reading the dataset.
Exploring the data to understand its structure.
Dropping any irrelevant or unwanted features that might not contribute to playlist creation.
### Modelling
The core of the project lies in applying the K-Means clustering algorithm to the audio features dataset. Before clustering, it's important to:
`Scale the data`: As features are on different scales, they need to be scaled to ensure equal importance.
Determine the optimal number of clusters using techniques like the Elbow Method and Silhouette Coefficient.
Once the optimal number of clusters is identified, the K-Means algorithm is applied to group songs into clusters.

## Cluster Exploration
After clustering, the resulting clusters need to be explored:

### Analyzing clusters' audio feature profiles.
Understanding the differences and similarities between clusters.
Potentially manually labeling clusters based on identified characteristics.

# Contributions
Apoorva Shandilya

Email: sshandilya90apoorva@gmail.com

Louise Dädlow

Email: galadaedlow@gmail.com

# Presentation
[Check this out](https://www.canva.com/design/DAFr-LwU_fo/R7EMDw_4DpHyRzaFN9y47g/view?utm_content=DAFr-LwU_fo&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)

# Conclusion
This project aims to demonstrate the feasibility of using unsupervised machine learning techniques to automate playlist creation. By leveraging audio features provided by Spotify, the project seeks to create clusters of songs that share similar traits. The success of this approach will be evaluated based on its ability to generate meaningful and cohesive playlists that align with Moosic's personalized and mood-based approach to curation.
