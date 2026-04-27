# Spotify Big Data Analytics

A music analytics and recommendation project built around large-scale audio feature extraction, metadata integration, MongoDB storage, and Spark-based similarity search.

This repository is best understood as a **music recommendation pipeline** that combines signal processing with big-data tooling.

## Problem this project solves

Music recommendation becomes harder when the dataset grows and when metadata alone is not enough to capture similarity. A stronger system needs to:

- extract useful audio features
- combine audio characteristics with metadata
- store processed representations efficiently
- search for similar tracks at scale

This project explores that workflow using Spotify-style music analytics and recommendation logic.

## What this project does

The pipeline:

- extracts audio features from music files
- combines them with track metadata
- stores processed results in MongoDB
- uses Apache Spark for large-scale similarity logic

The goal is to move from raw files and metadata to a system that can identify related tracks through feature-based search.

## Core components

### Audio feature extraction

The project extracts features such as:

- MFCCs
- spectral centroid
- zero-crossing rate
- track duration

### Data storage

Extracted features and metadata are stored in MongoDB so they can be queried and reused efficiently.

### Recommendation engine

The recommendation workflow uses Spark to:

- build feature vectors
- apply dimensionality reduction with PCA
- run nearest-neighbor style similarity search
- surface musically similar tracks

## Visual proof

![Spotify analytics preview](Screenshot%20from%202024-05-04%2016-35-07.png)

## Repository contents

- `phase1_extract_features.ipynb`: feature extraction notebook
- `MusicRecommendation.py`: recommendation logic
- `app.py`: application entry point
- `index.html`, `style.css`, `script.js`: front-end files

## Tech stack

- Python
- librosa
- MongoDB
- Apache Spark
- PCA and similarity search
- HTML, CSS, JavaScript

## Why this project matters

- It demonstrates audio feature engineering.
- It shows how data engineering and recommendation logic connect.
- It combines ML-style feature work with big-data infrastructure.
- It is useful for portfolio positioning in recommendation systems, analytics, and data pipelines.

## Typical local flow

1. prepare the audio dataset and metadata
2. run the extraction notebook
3. store feature outputs in MongoDB
4. launch the recommendation workflow
5. open the front-end interface if needed

## Industrial positioning

A more production-ready music recommendation pipeline would also need:

- scheduled ingestion of new content
- stronger metadata normalization
- evaluation metrics for recommendation quality
- online serving infrastructure
- latency and scale testing

This makes the repo best positioned as a **big-data music analytics and recommendation prototype**.
