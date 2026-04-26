# Spotify Big Data Analytics

A music analytics and recommendation project built around large-scale audio feature extraction, metadata integration, MongoDB storage, and Spark-based similarity search. The repository combines signal-processing ideas with big-data tooling to support music recommendation workflows.

## Overview

This project focuses on building a pipeline that:

- extracts audio features from music files
- combines them with track metadata
- stores the processed representations in MongoDB
- uses Apache Spark for large-scale recommendation logic

The overall goal is to move from raw audio and metadata to a system that can identify similar tracks through feature-based search.

## Project Components

### Audio Feature Extraction

The project extracts features such as:

- MFCCs
- spectral centroid
- zero-crossing rate
- track duration

These features provide a compact representation of each audio file for downstream similarity analysis.

### Data Storage

Extracted features and metadata are stored in a MongoDB collection so they can be queried, reused, and processed efficiently.

### Recommendation Engine

The recommendation system uses Spark to:

- build feature vectors
- apply dimensionality reduction with PCA
- run approximate nearest-neighbor search
- surface similar tracks based on audio characteristics

## Visual Proof

### Interface / Output Preview

![Spotify analytics preview](Screenshot%20from%202024-05-04%2016-35-07.png)

## Repository Contents

- `phase1_extract_features.ipynb`: feature extraction notebook
- `MusicRecommendation.py`: recommendation logic
- `app.py`: lightweight application entry point
- `index.html`, `style.css`, `script.js`: front-end interface files
- `Screenshot from 2024-05-04 16-35-07.png`: project preview image

## Tech Stack

- Python
- librosa
- MongoDB
- Apache Spark
- PCA / ANN-style similarity search
- HTML, CSS, JavaScript

## Why This Project Matters

This repository is a strong portfolio project because it demonstrates:

- audio feature engineering
- integration of signal processing with metadata pipelines
- NoSQL data storage
- large-scale recommendation thinking
- crossover between machine learning and big-data tooling

## Running the Project

The exact local setup depends on your MongoDB and Spark environment, but the typical flow is:

1. prepare the audio dataset and metadata
2. run the extraction notebook
3. store feature outputs in MongoDB
4. launch the recommendation logic
5. open the front-end files if using the browser-based interface

## Current Repository Status

This project is best understood as a preserved academic / portfolio pipeline rather than a polished production deployment. Its value is in the pipeline design, feature extraction workflow, and recommendation methodology.

## Author

Abubakar Shahid  
GitHub: <https://github.com/abubakarshahid16>
