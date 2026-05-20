# From Scratch Movie Recommender
![Python](https://img.shields.io/badge/Python-3.10-blue)

![TF-IDF](https://img.shields.io/badge/TF--IDF-From%20Scratch-orange)

![Cosine Similarity](https://img.shields.io/badge/Cosine-Similarity-green)

![NLP](https://img.shields.io/badge/NLP-Content%20Based-red)

![Datasets](https://img.shields.io/badge/Datasets-Movies%20%2B%20Credits-blue)

![Status](https://img.shields.io/badge/Status-Active-success)


A content-based movie recommendation system built completely from scratch using mathematical implementations of:

* TF (Term Frequency)
* IDF (Inverse Document Frequency)
* TF-IDF
* Cosine Similarity

This project does not use `TfidfVectorizer` or built-in cosine similarity libraries. The recommendation engine is manually implemented to understand the complete mathematics behind recommendation systems.

---

# Features

* Manual TF-IDF implementation
* Manual cosine similarity calculation
* Movie recommendation using content similarity
* TMDB 5000 movie dataset
* NLP preprocessing pipeline
* Genre, cast, keywords, crew, and overview based recommendations
* Stemming using NLTK
* Modular Python project structure

---

# Project Structure

```bash
from-scratch-movie-recommender/
│
├── main.py
├── preprocessing.py
├── tfidf_cosine.py
├── tmdb_5000_movies.csv
├── tmdb_5000_credits.csv
└── README.md
```

---

# Dataset

Datasets used:

- tmdb_5000_movies.csv
- tmdb_5000_credits.csv

These datasets were merged using the movie title column.

The datasets contain:

- Movie titles
- Genres
- Keywords
- Cast information
- Crew information
- Movie overviews
- Movie IDs

Note:

This project uses a subset of 500 movies from the TMDB 5000 dataset because TF-IDF and cosine similarity were implemented manually from scratch without optimized machine learning libraries.

---

# Technologies Used

* Python
* Pandas
* NLTK
* Math Module

---

# Recommendation Pipeline

```text
Dataset
   ↓
Preprocessing
   ↓
Create Tags
   ↓
TF Calculation
   ↓
IDF Calculation
   ↓
TF-IDF Vector Creation
   ↓
Cosine Similarity
   ↓
Top 5 Movie Recommendations
```

---

# Mathematical Formulas

## TF Formula

```text
TF = Count of Word in Document / Total Words in Document
```

## IDF Formula

```text
IDF = log(Total Documents / Documents Containing Word) + 1
```

## TF-IDF Formula

```text
TF-IDF = TF × IDF
```

## Cosine Similarity Formula

```text
Cosine Similarity = Dot Product / (Magnitude1 × Magnitude2)
```

---

# Preprocessing Steps

The preprocessing pipeline includes:

* Merging movie and credits datasets
* Extracting genres
* Extracting keywords
* Extracting top 3 cast members
* Extracting director names
* Removing spaces from names
* Converting overview into tokens
* Creating tags column
* Lowercasing text
* Applying stemming

---

# How to Run

## Install Required Libraries

```bash
pip install pandas nltk
```

---

## Run Project

```bash
python main.py
```

---

# Example

## Input

```text
Enter Movie Name: Avatar
```

## Output

```text
Top 5 Movies Similar to 'Avatar':

Guardians of the Galaxy -> 0.81
John Carter -> 0.77
Star Trek -> 0.74
Alien -> 0.72
Interstellar -> 0.70
```

---

# Why This Project Matters

Most beginner recommendation systems directly use:

```python
TfidfVectorizer()
cosine_similarity()
```

This project manually implements the complete mathematical logic behind recommendation systems.

The goal is not only to build a recommender system but also to deeply understand:

* NLP preprocessing
* Vectorization
* TF-IDF mathematics
* Similarity calculation
* Content-based filtering

---

# Future Improvements

Possible upgrades:

* Streamlit web app
* Flask API
* Collaborative filtering
* Word embeddings
* Deep learning recommendation system
* Hybrid recommendation engine
* Poster recommendation system
* Real-time search

---

# Author

Shivayya Sureban

---

# License

This project is open-source and available for educational purposes.

