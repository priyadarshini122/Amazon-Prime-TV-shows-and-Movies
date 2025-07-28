📊 Amazon Prime TV Shows and Movies – Exploratory Data Analysis (EDA)
🔍 Project Overview
This project focuses on performing Exploratory Data Analysis (EDA) on a dataset comprising TV shows and movies available on Amazon Prime Video. The dataset was created by merging two CSV files:

titles.csv: Contains information about each movie/show.

credits.csv: Contains information about people involved in the titles (like actors, directors, etc.).

The goal of this project is to understand the structure, trends, and key insights in the dataset using visualization and statistical techniques. No Machine Learning models are involved—this is strictly an EDA-focused project.

📁 Dataset Description
The merged dataset contains the following columns:

Column Name	Description
id	Unique identifier for each title
title	Name of the movie or TV show
type	Indicates whether it is a 'MOVIE' or a 'SHOW'
description	Summary of the title
release_year	Year of release
age_certification	Rating (e.g., PG-13, TV-MA)
runtime	Duration in minutes
genres	Genre(s) associated (e.g., Comedy, Drama)
production_countries	Country where the title was produced
seasons	Number of seasons (for shows only)
imdb_id	IMDb identifier
imdb_score	IMDb rating
imdb_votes	Number of IMDb votes
tmdb_popularity	Popularity score from TMDB
tmdb_score	TMDB rating
person_id	Person identifier (actors, directors, etc.)
name	Name of the person
character	Character name (for actors)
role	Role in the production (e.g., Actor, Director)

🧹 Data Cleaning
Dropped rows with missing description.

Replaced missing values in numerical columns (like imdb_score, tmdb_score) with the mean.

Replaced missing categorical fields (age_certification, character) with mode or placeholder values.

Filled missing season counts with 0.

Checked and removed duplicates.

📈 Exploratory Data Analysis (EDA)
✅ Univariate Analysis
Box plots for imdb_score, runtime

Histograms for release_year, runtime, seasons, imdb_score

Bar charts for type, age_certification, genres, production_countries

✅ Bivariate Analysis
Scatter plot: imdb_votes vs imdb_score

Line plots: Trend of runtime, seasons, and imdb_score over years

Violin plot: imdb_score by type

Heatmap: Correlation between numeric variables

✅ Pie Charts
Distribution of type (Movies vs Shows)

Distribution of age_certification

💡 Key Insights
Most content is categorized as "MOVIES".

PG-13 and TV-MA are the most common age certifications.

Genres like Drama, Comedy, and Action dominate the platform.

Countries like United States and India are major production hubs.

IMDB scores mostly lie between 6.0 and 8.0, with a few outliers.

There’s a positive correlation between imdb_votes and imdb_score.

🎯 Project Conclusion
This EDA project successfully uncovers key insights about the content hosted on Amazon Prime Video. The visualizations help understand content trends over the years, preferred genres, audience ratings, and more. These insights can support data-driven decisions in content acquisition, customer targeting, and platform optimization.

🛠️ Tools Used
Python

Pandas

Matplotlib

Seaborn

Plotly (for interactive pie charts)

Jupyter Notebook / Google Colab

📌 Author
Name: Priya Darshini
Email: priyadarshinigaddala52@gmail.com
Batch: 15 July
Domain: Data Analytics
