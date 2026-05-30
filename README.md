# Movie Recommendation System with Sentiment Analysis







## 🎬 Advanced Content-Based Filtering & NLP

This project is a high-performance recommendation engine that suggests movies based on content similarity and utilizes **Natural Language Processing (NLP)** to analyze user sentiment from reviews in real-time. It bridges the gap between raw data science models and a functional web application.

---

## 🛠️ Deep Technical Dive

### 1. The Recommendation Logic (Cosine Similarity)
The system represents each movie as a vector based on features like **Genres, Cast, Director, and Keywords**. To find similar movies, it calculates the **Cosine Similarity** between these vectors.

$$\text{similarity} = \cos(\theta) = \frac{\mathbf{A} \cdot \mathbf{B}}{\|\mathbf{A}\| \|\mathbf{B}\|}$$

* **Closer to 1:** Movies are highly similar.
* **Closer to 0:** Movies are unrelated.

### 2. NLP & Sentiment Analysis
The sentiment analysis engine uses a **Multinomial Naive Bayes** classifier. It processes user reviews through a specific pipeline:
* **Tokenization:** Breaking down sentences into individual words.
* **Stop-word Removal:** Filtering out common words that don't carry sentiment.
* **Vectorization:** Converting text into a numerical format using `transform.pkl`.

---

## 📂 Project Structure

* `main.py`: The **Flask** backend handling routes and model inference.
* `preprocessing.ipynb`: Data wrangling scripts for merging the TMDB 5000 dataset.
* `sentiment.ipynb`: The training logic for the sentiment analysis model.
* `nlp_model.pkl` & `transform.pkl`: Serialized models for fast, real-time inference.
* `static/`: Contains `content.js` and CSS for the dynamic frontend.
* `templates/`: HTML structures for the user interface.

---

## 🚀 Getting Started

To run this project locally, follow these steps:

### 1. Clone the Repository
```bash
git clone [https://github.com/Ayushi22jain/Movie-Recommendation-System.git](https://github.com/Ayushi22jain/Movie-Recommendation-System.git)
cd Movie-Recommendation-System

### 2. Install Dependencies
```bash
pip install -r requirements.txt

python main.py


Open http://127.0.0.1:5000/ in your browser.

## 📈 Key Features
Real-time Suggestions: Instant movie recommendations based on metadata similarity.

Sentiment Analysis: Automatically detects the tone of reviews to help users decide what to watch.

AJAX Integration: Seamlessly fetches data from the backend without page refreshes.

End-to-End Pipeline: Covers everything from data cleaning to a deployed web UI.

## 🔗 Author
Ayushi Jain

GitHub: Ayushi22jain
