# Anime Recommendation System Using Cosine Similarity

## Objective

The objective of this project is to build an anime recommendation system using
Cosine Similarity. The system recommends anime titles that are similar to a
given anime based on selected features such as genres, ratings, and other
relevant attributes.

## Dataset

The dataset used in this project is `anime.csv`.

The dataset contains information about various anime titles, including:

- Anime ID
- Anime title
- Broadcast type
- Genre
- Number of episodes
- Average user rating
- Number of community members

## Project Workflow

### 1. Data Preprocessing

The following preprocessing steps were performed:

- Loaded the dataset using Pandas.
- Explored the structure and attributes of the dataset.
- Checked for missing values.
- Handled missing values appropriately.
- Checked for duplicate records.
- Prepared categorical and numerical features for similarity analysis.

### 2. Feature Extraction

Relevant features were selected for calculating similarity between anime titles.

The selected features may include:

- Genre
- Rating
- Number of episodes
- Other relevant anime attributes

Categorical features were converted into numerical representations where
necessary.

Numerical features were normalized when required so that features with larger
scales did not dominate the similarity calculation.

### 3. Cosine Similarity

Cosine Similarity was used to measure the similarity between anime titles.

Cosine similarity measures the angle between two feature vectors. A higher
similarity score indicates that two anime titles have more similar
characteristics.

### 4. Recommendation System

A recommendation function was created that:

- Accepts an anime title as input.
- Finds the corresponding feature representation.
- Calculates similarity with other anime titles.
- Sorts anime based on similarity scores.
- Returns the most similar anime recommendations.

### 5. Similarity Threshold

Different similarity threshold values were experimented with to understand
their effect on the number of recommendations.

A higher threshold produces recommendations that are more similar to the
selected anime, while a lower threshold can provide a larger and more diverse
recommendation list.

### 6. Recommendation Analysis

The recommendation results were analyzed to determine:

- Whether the recommended anime are relevant to the selected title.
- How similarity scores affect recommendations.
- How feature selection influences recommendation quality.
- Possible improvements to the recommendation system.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## Project Structure

```text
Anime-Recommendation-System-Using-Cosine-Similarity/
│
├── Anime_Recommendation_System.ipynb
├── anime.csv
└── README.md
