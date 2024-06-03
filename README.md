# Movie Recommendation System

This is a simple content based movie recommendation system built using Python and machine learning techniques. It recommends movies to users based on similarities in their tags, which include movie overview, genres, keywords, cast, and crew.

---
## Dataset

The system uses the TMDb (The Movie Database) dataset, which contains information about thousands of movies. It includes details such as movie title, overview, genres, keywords, cast, and crew.

- **tmdb_5000_movies.csv**
- **tmdb_5000_credits.csv**

## Preprocessing

Before building the recommendation system, the dataset needs to be preprocessed as :

- Merging the movies and credits dataframes on the movie title.
- Selecting relevant features such as movie ID, title, overview, genres, keywords, cast, and crew.
- Converting textual data into usable format (e.g., converting JSON strings to lists).

## Recommendation Algorithm

The recommendation algorithm is based on cosine similarity between movies. It calculates the similarity scores for each pair of movies based on their tags (overview, genres, keywords, cast, and crew) using the CountVectorizer and cosine_similarity functions from scikit-learn.

## Usage

To use the movie recommendation system:

1. Ensure you have Python installed on your system or you can utilize jupyter on browser.
2. Install the required libraries.
3. Download the TMDb dataset files (`tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`).
4. Run the `recommend()` function in Python, passing the title of the movie for which you want recommendations.

```python
recommend(Enter Movie Name Here)
```

## Input
```python
recommend('Gandhi')
```
## Output
```python
Gandhi, My Father
The Wind That Shakes the Barley
A Passage to India
Guiana 1838
Ramanujan
```
## Input
```python
recommend('Abhjasd')
```
## Output
```python
Movie not found.
```
