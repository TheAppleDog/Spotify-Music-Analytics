# What Makes a Hit? | Spotify Music Analytics with Tableau 🎧

## 📌 Project Overview
This project explores Spotify track data to investigate how track popularity varies across genres, artists, and audio characteristics.

The analysis focuses on popularity, danceability, energy, valence, acousticness, instrumentalness, and track duration.

**Main question:** Which genres, artists, and audio characteristics are associated with higher track popularity in this dataset?

## 🎯 Business Questions
- Which genres have the highest average popularity?
- Which artists and tracks rank highly by popularity?
- How is popularity distributed across tracks?
- What relationships can be observed between popularity and danceability, energy, or valence?
- How do audio characteristics vary across genres?
- How can users explore different audio metrics interactively?

## 🛠️ Tools & Techniques
- Tableau
- Spotify Tracks Dataset
- Data exploration and visualization
- Calculated fields and KPI development
- Interactive filters
- Parameters and dynamic metric selection
- Scatter plots and genre comparisons

## 📊 Dashboards

### 1. Music Overview
Summarizes the dataset using:
- Total Tracks
- Average Popularity
- Average Danceability
- Average Energy
- Popularity by Genre
- Artist Popularity
- Popularity Tier Distribution
- Top 10 Tracks by Popularity

Interactive filters allow users to explore the data by genre, artist, and popularity tier.

### 2. What Makes a Hit?
Investigates relationships between popularity and audio characteristics using:
- Average Popularity
- Average Danceability
- Average Energy
- Average Track Duration
- Danceability versus Popularity
- Energy versus Popularity
- Valence versus Popularity
- Audio-feature comparisons
- A dynamic parameter to select an audio metric

## 🧮 Key Calculations

**Duration in Minutes**
```text
[duration_ms] / 60000
```

**Popularity Tier**
```text
IF [popularity] >= 75 THEN "Hit"
ELSEIF [popularity] >= 50 THEN "Popular"
ELSEIF [popularity] >= 25 THEN "Emerging"
ELSE "Niche"
END
```

**Energy Level**
```text
IF [energy] >= 0.75 THEN "High Energy"
ELSEIF [energy] >= 0.50 THEN "Medium Energy"
ELSE "Low Energy"
END
```

**Mood Profile**
```text
IF [valence] >= 0.65 THEN "Positive"
ELSEIF [valence] >= 0.35 THEN "Neutral"
ELSE "Melancholic"
END
```

## 💡 Analytical Approach
The dashboards enable comparisons between popularity and audio characteristics, helping users explore patterns across genres and tracks.

Observed relationships should be treated as associations, not proof that a particular audio feature causes a track to become popular. Popularity can also depend on factors outside the dataset.

## 📷 Dashboard Screenshots
Add screenshots of both completed dashboards here.

Suggested filenames:
- `music-overview.png`
- `what-makes-a-hit.png`

## 📁 Dataset
Spotify Tracks Dataset: https://github.com/sai-chaitanya-reddy/spotify-tracks-dataset

Please verify the dataset description and source details against the version used in this project.

## ⚠️ Limitations
This project explores the available track data and does not establish why a song becomes popular. The dataset does not provide geographic fields for a geographic analysis.

## 👩‍💻 Project Type
Self-directed Data Analytics portfolio project.

## 🏷️ Skills
Tableau · Data Analytics · Data Visualization · Calculated Fields · Interactive Dashboards · Exploratory Data Analysis
