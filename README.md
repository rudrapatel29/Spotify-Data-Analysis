# Spotify Data Analysis

## Overview
This project aims to analyze a dataset of Spotify music tracks to uncover trends, patterns, and insights related to track popularity, genre distribution, and various musical attributes. The analysis involves data cleaning, exploration, visualization, and statistical analysis to provide comprehensive insights into the music industry.

## Project Goals
- **Popularity Analysis**: Investigate the popularity of tracks over time and identify the top genres based on popularity.
- **Genre Analysis**: Determine the most popular genres and analyze their characteristics.
- **Audio Features Exploration**: Examine various audio features like danceability, energy, loudness, and more to understand their impact on track popularity.

### Datasets

This project uses two datasets:

1. **Spotify Features**
   - Purpose: Provides detailed audio features and metadata for tracks, which are essential for exploring correlations between audio features and track popularity.
   
2. **Tracks**
   - Purpose: Offers comprehensive data on track popularity, artists, and release dates, which are crucial for analyzing trends over time and across genres.

### Spotify Features

| Column          | Description                             | Data Type     |
| :-------------- | :-------------------------------------- | :------------ |
| genre           | Genre of the track                      | VARCHAR       |
| artist_name     | Name of the artist                      | VARCHAR       |
| track_name      | Name of the track                       | VARCHAR       |
| track_id        | Unique identifier for the track         | VARCHAR       |
| popularity      | Popularity score of the track           | INT           |
| acousticness    | Measure of the acoustic quality         | FLOAT         |
| danceability    | Measure of how suitable a track is for dancing | FLOAT    |
| duration_ms     | Duration of the track in milliseconds   | INT           |
| energy          | Measure of intensity and activity       | FLOAT         |
| instrumentalness| Measure of the instrumental quality     | FLOAT         |
| key             | Key in which the track is composed      | INT           |
| liveness        | Presence of a live audience             | FLOAT         |
| loudness        | Overall loudness of the track           | FLOAT         |
| mode            | Modality of the track (major or minor)  | INT           |
| speechiness     | Presence of spoken words                | FLOAT         |
| tempo           | Tempo of the track                      | FLOAT         |
| time_signature  | Time signature of the track             | INT           |
| valence         | Measure of the musical positiveness     | FLOAT         |

### Tracks

| Column          | Description                             | Data Type     |
| :-------------- | :-------------------------------------- | :------------ |
| id              | Unique identifier for the track         | VARCHAR       |
| name            | Name of the track                       | VARCHAR       |
| popularity      | Popularity score of the track           | INT           |
| duration_ms     | Duration of the track in milliseconds   | INT           |
| explicit        | Indicates if the track contains explicit content | BOOLEAN   |
| artists         | List of artists for the track           | VARCHAR       |
| id_artists      | Unique identifiers for the artists      | VARCHAR       |
| release_date    | Release date of the track               | DATE          |
| danceability    | Measure of how suitable a track is for dancing | FLOAT    |
| energy          | Measure of intensity and activity       | FLOAT         |
| key             | Key in which the track is composed      | INT           |
| loudness        | Overall loudness of the track           | FLOAT         |
| mode            | Modality of the track (major or minor)  | INT           |
| speechiness     | Presence of spoken words                | FLOAT         |
| acousticness    | Measure of the acoustic quality         | FLOAT         |
| instrumentalness| Measure of the instrumental quality     | FLOAT         |
| liveness        | Presence of a live audience             | FLOAT         |
| valence         | Measure of the musical positiveness     | FLOAT         |
| tempo           | Tempo of the track                      | FLOAT         |
| time_signature  | Time signature of the track             | INT           |

## Unique columns in each dataset:

### Spotify Features
- `genre`
- `artist_name`
- `track_name`
- `track_id`

### Tracks
- `id`
- `explicit`
- `artists`
- `id_artists`
- `release_date`

## Data Wrangling and Manipulation
The following techniques were used to clean and manipulate the dataset:
- **Handling Missing Values**: Identified and removed rows with missing values in critical columns like `name`.
- **DateTime Conversion**: Converted the `release_date` column to datetime format to facilitate time-based analysis.
- **Indexing**: Set the `release_date` column as the index for easier time series analysis.
- **Feature Extraction**: Extracted the year from the `release_date` to analyze trends over time.

## Analysis Highlights
### Data Cleaning
- Identified and removed rows with missing values in critical columns like `name`.

### Popularity Analysis
- Analyzed the top 5 genres by popularity using bar plots.
- Visualized average popularity by genre to identify the most popular genres over time.
- Examined trends in track popularity over the years.

### Audio Features Exploration
- Investigated the relationship between various audio features and track popularity.
- Created scatter plots, bar charts, and heatmaps to visualize correlations and patterns.

## Visualization and Tools
### Libraries Used
- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations.
- `matplotlib`: For plotting and visualization.
- `seaborn`: For advanced visualizations.

### Visualization Techniques
- **Bar plots**: To show top genres and average popularity.
- **Line plots**: To visualize trends over time.
- **Scatter plots and heatmaps**: To explore correlations between audio features and popularity.

## PowerBI Dashboard
The PowerBI dashboard includes the following visualizations:
- **Artists with Most Album Releases**: Bar chart of the top 13 artists with the most album releases.
- **Popularity by Genre**: Pie chart depicting the distribution of music popularity across various genres.
- **Average Popularity by Speechiness**: Scatter plot showing the relationship between speechiness and average popularity.
- **Top 10 Artists with Most Explicit Songs**: Bar chart of the top 10 artists with the most explicit songs.
- **Average Duration of Songs over a Century**: Line graph showing the trend in average song duration over time.
- **Artists**: List of various artists.

## Conclusion
This project provides valuable insights into the music industry by analyzing track popularity, genre distribution, and audio features. The findings can help music producers, artists, and enthusiasts understand trends and factors contributing to a track's success.

## Repository Contents
- **Data**: The dataset used for analysis (with necessary anonymization and data cleaning steps).
- **Notebooks**: Jupyter notebooks containing the data analysis and visualization code.
- **Scripts**: Python scripts for data processing and analysis.
- **Results**: Visualizations and findings from the analysis.

## Findings and Visualizations
- **Top 5 Records By Popularity**
- **Number of Tracks with Popularity Greater Than a Certain Threshold**
- **Top 10 Most Popular Tracks**
- **Top 10 Least Popular Tracks**
- **Relationship between Loudness and Energy**
- **Relationship between Popularity and Acoustics**
- **Correlation Between Variables**
- **Duration of Songs over the Years**
- **Average Popularity by Genre**
- **Number of Songs per Year**
- **Duration of Songs across Different Genres**
