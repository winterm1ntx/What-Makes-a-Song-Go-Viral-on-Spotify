# 🎵 What Makes a Song Go Viral on Spotify?
End-to-end analysis of 97,149 Spotify tracks to identify what factors drive song popularity — covering genre, audio features, and content type.

# 📌 Overview
This project analyzes the Spotify Tracks Dataset to answer a core question: what makes a song go viral on Spotify? The analysis covers the full data analytics workflow — from data cleaning and exploratory analysis to statistical correlation and interactive Tableau dashboard.

# ❓ Research Questions
1.  What does the distribution of song popularity look like — how rare are truly viral songs?

2.  Which genres consistently produce the most popular songs?

3.  Which audio features correlate most with popularity?

4.  Do explicit songs tend to be more popular than non-explicit ones?

# 📂 Dataset
•  Source: Spotify Tracks Dataset (Kaggle)
•  Raw records: 114,000 tracks across 114 genres
•  After cleaning: 97,149 tracks
## Cleaning criteria:
•  Removed 3 rows with null values

•  Removed tracks with duration of 0ms

•  Removed tracks with popularity score of 0 (likely never played)
    
•  Removed duplicates
•  Selected 11 relevant columns for analysis

Note: This dataset contains exactly 1,000 tracks per genre by design, which should be considered when interpreting statistical results.

# 🔧 Tools & Tech Stack
•  Data Processing: Python (pandas)
•  Visualization: matplotlib, seaborn, Tableau
•  Statistical Analysis: scipy (Pearson correlation)
•  Notebook: Jupyter Notebook

# 📊 Key Findings
Popularity Distribution — Only 5.6% of active tracks reach viral status (popularity ≥ 70). Most songs cluster in the 20–60 range.

Genre — Pop, pop-film, and k-pop lead in average popularity, but the gap between genres is very small — genre alone is not a reliable predictor of popularity.

Audio Features — No audio feature shows a strong correlation with popularity. Loudness and danceability have the highest positive correlation (+0.07), but the relationship is too weak to be actionable.

Explicit Content — Explicit songs score slightly higher on average (42.1 vs 38.4), but the difference is not significant enough to be a deciding factor.

# 💡 Key Insight
Going viral on Spotify is not about how a song sounds technically. Popularity is likely driven more by factors outside this dataset — such as artist reputation, marketing strategy, and platform recommendation algorithms.

# ✅ Recommendations
•  Do not rely on audio formulas to predict viral success — danceability, energy, and tempo have negligible impact on popularity.

•  Genre is not a reliable predictor — choosing pop or k-pop does not guarantee higher popularity.

•  Focus on factors outside the data — artist reputation, quality of songwriting, and promotion strategy likely matter more than audio characteristics alone.

# 📁 File Structure
├── spotify_viral_analysis.ipynb   # Main notebook (cleaning, EDA, correlation)
├── spotifity_fix.twbx             # Dashboard File
├── README.md                      # Project documentation
