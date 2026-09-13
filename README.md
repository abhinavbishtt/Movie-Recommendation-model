A machine learning-based Movie Recommendation System that suggests similar movies based on user preferences and movie features. Built using Python, Pandas, NumPy, and Scikit-learn,  for quick and personalized recommendations.
# 🎬 Movie Recommendation System

A **Content-Based Movie Recommendation System** built using Python and Machine Learning techniques. The system recommends movies based on the similarity between their metadata such as overview, genres, keywords, and tagline.

## 📌 Project Overview

This project uses a movie dataset to build a recommendation model that finds movies similar to a movie selected by the user.

The recommendation system uses **CountVectorizer** to convert movie metadata into numerical vectors and **Cosine Similarity** to calculate the similarity between movies.

> **Note:** This project currently contains the Python recommendation model and does not include a graphical user interface or web application.

## ⚙️ How It Works

The model follows these main steps:

1. Load the movie dataset.
2. Select relevant movie features such as:

   * Overview
   * Genres
   * Keywords
   * Tagline
3. Combine these features into a single `tags` column.
4. Apply **stemming** using NLTK's Porter Stemmer.
5. Convert the text into numerical vectors using **CountVectorizer**.
6. Calculate similarity between movies using **Cosine Similarity**.
7. Return the top 5 movies most similar to the selected movie.

## 🧠 Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* NLTK
* Jupyter Notebook

## 🤖 Machine Learning Techniques

### CountVectorizer

`CountVectorizer` converts the movie text data into numerical vectors based on the frequency of words.

### Cosine Similarity

Cosine similarity is used to measure how similar two movie vectors are. Movies with higher similarity scores are considered more similar.

### Porter Stemmer

NLTK's `PorterStemmer` is used to reduce words to their root form, helping the model identify similar words.

## 🔍 Example

For example:

```python
recommend('Avatar')
```

The model generates recommendations such as:

```text
Titan A.E.
Battle: Los Angeles
Small Soldiers
The Fifth Element
The 5th Wave
```

## 📂 Project Structure

```text
Movie-Recommendation/
│
├── Untitled.ipynb
├── README.md
└── dataset files
```

## 🚀 Future Improvements

* Build a Streamlit web interface
* Add movie posters and additional movie information
* Improve recommendation accuracy
* Deploy the application online
* Add a search-based user interface

## 👨‍💻 Project Status

**Completed:** Content-based movie recommendation model

**Future:** User interface and web deployment

## 📄 License

This project is created for educational and learning purposes.
