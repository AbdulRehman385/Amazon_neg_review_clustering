# Amazon Music Reviews Analysis

## Project Overview

This project analyzes negative reviews from the [Amazon Music Reviews dataset](https://www.kaggle.com/datasets/eswarchandt/amazon-music-reviews) to identify recurring patterns and issues with music accessories and instruments. Using **Natural Language Processing (NLP)** and **clustering techniques**, the project aims to group negative reviews into actionable themes, providing insights to improve product quality and customer satisfaction.

---

## Workflow

1. **Data Preprocessing**
   - Removed URLs, emojis, punctuation, and extra spaces.
   - Converted text to lowercase.
   - Applied lemmatization using `spaCy`.

2. **Sentiment Analysis**
   - Used the `SentimentIntensityAnalyzer` to identify negative reviews.

3. **Feature Extraction**
   - Applied `TfidfVectorizer` to transform the text into numerical features.

4. **Clustering**
   - Determined the optimal number of clusters using the silhouette score.
   - Applied the K-means algorithm for clustering negative reviews.

---

## Results

The analysis produced **seven clusters** of recurring themes in the reviews:

- **Cluster 0**: Sound quality and connectivity issues (e.g., cables, devices, amplifiers).
- **Cluster 1**: Complaints about guitar straps (e.g., durability, compatibility).
- **Cluster 2**: Issues with guitar picks, cases, and bass accessories.
- **Cluster 3**: Problems with tuners (e.g., battery life, display accuracy).
- **Cluster 4**: Functional and durability concerns with pedals and cables.
- **Cluster 5**: Stability and usability complaints about stands and mounts.
- **Cluster 6**: Concerns about guitar strings, tone, tuning, and fret quality.

---

## Key Insights

- The clustering reveals specific problem areas for manufacturers and sellers.
- Quality control, better product design, and improved user support can address many of these issues.

---

## Tools and Libraries

- **Python**: Data processing and analysis
- **spaCy**: Text preprocessing
- **NLTK**: Sentiment analysis
- **Scikit-learn**: Vectorization, clustering, and evaluation
