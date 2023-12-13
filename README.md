# Movie-Recommendation-System---Sritesh-Suranjan

# Movie Recommendation System

## Overview

This project implements a movie recommendation system using content-based filtering. It leverages natural language processing (NLP) techniques and cosine similarity to recommend movies based on their textual content, specifically the combination of movie overviews and genres.

## Table of Contents

- [Introduction](#introduction)
- [Data](#data)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Preprocessing](#data-preprocessing)
- [Text Vectorization](#text-vectorization)
- [Similarity Calculation](#similarity-calculation)
- [Movie Recommendations Function](#movie-recommendations-function)
- [Example Recommendations](#example-recommendations)
- [Model Saving and Loading](#model-saving-and-loading)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Movie Recommendation System uses content-based filtering to recommend movies based on their textual information, combining movie overviews and genres. It employs natural language processing (NLP) techniques and cosine similarity to determine movie similarity.

## Data

The dataset (`top10K-TMDB-movies.csv`) contains information about movies, including `id`, `title`, `overview`, and `genre`.

## Exploratory Data Analysis

The initial exploration involves displaying the first 10 rows, generating summary statistics, and checking for null values.

## Data Preprocessing

Data preprocessing includes selecting relevant columns (`id`, `title`, `overview`, `genre`), creating a new column `tags` by concatenating `overview` and `genre`, and dropping irrelevant columns (`overview`, `genre`).

## Text Vectorization

Text vectorization is performed using `CountVectorizer` from `sklearn.feature_extraction.text` to convert text data into numerical vectors.

## Similarity Calculation

Cosine similarity is calculated based on the vectorized tags, creating a similarity matrix.

## Movie Recommendations Function

A function named `recommends` is defined to recommend movies based on user input.

## Example Recommendations

An example demonstrates recommending movies for a specific input movie title, such as "Iron Man."

## Model Saving and Loading

The processed data (`new_data`) and the similarity matrix are saved using the `pickle` module. Loading the model back into the program is also demonstrated.

## Dependencies

- Python 3.x
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn

## Usage

1. Install the required dependencies: `pip install -r requirements.txt`
2. Run the Python script or Jupyter notebook.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

This project is licensed under the [MIT License](LICENSE).
