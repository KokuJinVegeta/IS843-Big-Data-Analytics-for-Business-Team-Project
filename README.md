# Level Up: Turning Player Voices into Game Development Insights
# Analysis of 51M Steam Reviews & 1GB+ Game Metadata

## A QST843 Big Data Analytics for Business Project

## Overview

This project demonstrates how large-scale Steam player reviews can be transformed into insights that help developers build better games. The notebook analyzes:
* 51M+ reviews
* 1GB+ game metadata
* 100,000+ unique game titles

The goal is to make sense of massive, unstructured user feedback and extract actionable patterns related to sentiment, engagement, game features, and publisher behavior.

You’ll find the full analysis here:
_QST7-Level-Up-Player-Reviews-For-Development.ipynb_

The notebook contains code, documentation, feature engineering steps, sentiment aggregation, and visualizations.

## Data Sources
The analysis uses two large datasets (referenced via Google Cloud Storage):

all_reviews.csv — player reviews (~51M rows)

games.csv — game metadata (tags, release year, publishers, etc.)

These datasets are not included due to size but the notebook shows complete ETL and merging steps using PySpark.

## Data Engineering
* Large-scale data ingestion with PySpark
* Review cleaning (English filtering, deduplication, timestamp normalization)
* Game metadata cleanup and merging
* Feature Engineering
* Sentiment labels (voted_up)
* Word count metrics
* Playtime bands
* Game tag parsing
* Publisher-level aggregations
* Insight Generation

## The notebook identifies trends such as:
* Which publishers receive the highest/lowest player sentiment
* How playtime and sentiment interact
* What tags or genres correlate with positive/negative reviews
* Longitudinal sentiment trends over time

## Intended Users
This project will be useful for:
* Game developers
* Data scientists analyzing textual or behavioral datasets
* Students exploring large-scale analytics
* Industry analysts researching Steam ecosystem trends

## Running the Analysis
Requirements
* PySpark 3.5+
* Google Cloud Dataproc (recommended)
* Python packages: pandas, matplotlib, seaborn

## Instructions
1. Upload datasets to your storage location (e.g., GCS).
2. Update file paths in the notebook if required.
3. Run ETL cells first — they prepare the full dataset.
4. Proceed into sentiment trends, aggregations, and plots.
5. Extend or repurpose the notebook for additional modeling (topic modeling, embeddings, clustering).

##Future Enhancements
Potential additions:
* NLP topic modeling (LDA, BERTopic)
* Transformer-based sentiment classification
* Time-series forecasting of review trends
* Interactive dashboards for developer teams
* Embeddings for deeper semantic understanding

## Project Contributors
Lucien Williams
Rhea Desai
Vanessa Sung
Wenlin (Tina) Zhao

## License
This project is for academic and non-commercial use.
