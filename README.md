# Spotify Music Tracks Data Analysis

## Overview
This project aims to analyze a dataset of Spotify music tracks to uncover trends, patterns, and insights related to track popularity, genre distribution, and various musical attributes. The analysis involves data cleaning, exploration, visualization, and statistical analysis.

## Project Goals
- **Popularity Analysis**: Investigate the popularity of tracks over time and identify the top genres based on popularity.
- **Genre Analysis**: Determine the most popular genres and analyze their characteristics.
- **Audio Features Exploration**: Examine various audio features like danceability, energy, loudness, and more to understand their impact on track popularity.

## Dataset
The dataset used in this project includes the following columns:
- `id`: Unique identifier for the track
- `name`: Name of the track
- `popularity`: Popularity score of the track
- `duration_ms`: Duration of the track in milliseconds
- `explicit`: Indicates if the track contains explicit content
- `artists`: List of artists for the track
- `id_artists`: Unique identifiers for the artists
- `release_date`: Release date of the track
- `danceability`: Measure of how suitable a track is for dancing
- `energy`: Measure of intensity and activity
- `key`: Key in which the track is composed
- `loudness`: Overall loudness of the track
- `mode`: Modality of the track (major or minor)
- `speechiness`: Presence of spoken words in the track
- `acousticness`: Measure of the acoustic quality of the track
- `instrumentalness`: Measure of the instrumental quality of the track
- `liveness`: Presence of a live audience in the track
- `valence`: Measure of the musical positiveness of the track
- `tempo`: Tempo of the track
- `time_signature`: Time signature of the track

## Data Wrangling and Manipulation
The following techniques were used to clean and manipulate the dataset:
- **Handling Missing Values**: Identified and removed rows with missing values in critical columns like `name`.
- **DateTime Conversion**: Converted the `release_date` column to datetime format to facilitate time-based analysis.
- **Indexing**: Set the `release_date` column as the index for easier time series analysis.
- **Feature Extraction**: Extracted the year from the `release_date` to analyze trends over time.

## Analysis Highlights
- **Data Cleaning**: Identified and removed rows with missing values in critical columns like `name`.
- **Popularity Analysis**:
  - Analyzed the top 5 genres by popularity using bar plots.
  - Visualized average popularity by genre to identify the most popular genres over time.
  - Examined trends in track popularity over the years.
- **Audio Features Exploration**:
  - Investigated the relationship between various audio features and track popularity.
  - Created scatter plots, bar charts, and heatmaps to visualize correlations and patterns.

## Visualization and Tools
- **Libraries Used**:
  - `pandas`: For data manipulation and analysis
  - `numpy`: For numerical operations
  - `matplotlib`: For plotting and visualization
  - `seaborn`: For advanced visualizations
- **Visualization Techniques**:
  - Bar plots to show top genres and average popularity.
  - Line plots to visualize trends over time.
  - Scatter plots and heatmaps to explore correlations between audio features and popularity.

## Conclusion
This project provides valuable insights into the music industry by analyzing track popularity, genre distribution, and audio features. The findings can help music producers, artists, and enthusiasts understand trends and factors contributing to a track's success.

## Repository Contents
- **Data**: The dataset used for analysis (with necessary anonymization and data cleaning steps).
- **Notebooks**: Jupyter notebooks containing the data analysis and visualization code.
- **Scripts**: Python scripts for data processing and analysis.
- **Results**: Visualizations and findings from the analysis.

## Findings and Visualizations
- Top 5 Records By Popularity
- Number of Tracks that have popularity greater than a certain threshold
- Top 10 most popular tracks with popularity
- Top 10 least popular tracks
- Relationship between Loudness and Energy
- Relationship between Popularity and Acoustics
- Correlation Between Variables
- Duration of Songs over the Years
- Average Popularity by Genre
- Number of Songs per Year
- Duration of Songs across Different Genres
