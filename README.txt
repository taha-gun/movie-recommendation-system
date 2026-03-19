# Movie Recommendation System

This project implements collaborative filtering techniques to build a movie recommendation system using the MovieLens dataset.

Two approaches are implemented:
- Item-Based Collaborative Filtering
- User-Based Collaborative Filtering

## Overview

The goal of this project is to understand and implement recommendation system logic using real-world user rating data.

- Item-based filtering recommends movies similar to a selected movie  
- User-based filtering recommends movies based on similar users’ preferences  

## Methods

### Item-Based Collaborative Filtering
- Uses Pearson correlation to measure similarity between movies  
- Recommends movies based on item-to-item relationships  
- Applies a minimum rating threshold to reduce noisy correlations  

### User-Based Collaborative Filtering
- Uses cosine similarity to identify similar users  
- Generates recommendations using weighted user ratings  
- Filters low-signal recommendations using rating count thresholds  

## Tech Stack

- Python  
- Pandas  
- NumPy  
- Scikit-learn  

## Dataset

- MovieLens dataset (user ratings and movie metadata)

## Project Structure

```text
movie-recommendation-system/
├── data/
│   ├── movies.csv
│   └── ratings.csv
├── notebooks/
│   ├── item_based_recommendation.ipynb
│   └── user_based_recommendation.ipynb
├── README.md
└── requirements.txt
'''
## How to Run

1. Place `movies.csv` and `ratings.csv` inside the `data/` folder  
2. Open the notebooks inside the `notebooks/` directory  
3. Run all cells in order  

Make sure required libraries are installed:

```bash
pip install -r requirements.txt
```

## Key Learnings

- Handling sparse user-item matrices  
- Understanding similarity metrics (Pearson vs Cosine)  
- Applying thresholding to improve recommendation quality  
- Building end-to-end recommendation pipelines  

## Status

Project is actively being improved.
