# Movie Recommendation System with Sentiment Analysis

This project is a full-stack recommendation engine that suggests movies based on content similarity and performs sentiment analysis on user reviews. By combining NLP techniques with similarity metrics, the system provides a personalized and interactive movie discovery experience.

---

## 📂 Project Structure
* **`main.py`**: The core application script handling the backend logic.
* **`preprocessing.ipynb`**: Detailed data cleaning and feature engineering notebooks.
* **`sentiment.ipynb`**: Implementation of the NLP sentiment analysis model.
* **`nlp_model.pkl` & `tranform.pkl`**: Serialized models for fast inference.
* **`home.html` & `recommend.html`**: Web interface for the user-facing application.

---

## 🛠️ How It Works

### 1. Recommendation Engine (Content-Based)
* **Similarity Metric:** Uses **Cosine Similarity** to calculate the distance between movie vectors based on genres, cast, and plot keywords.
* **Data Processing:** Merges multiple datasets (`movie_metadata.csv`, `data.csv`) to create a robust feature set for the recommender.

### 2. Sentiment Analysis
* **Natural Language Processing (NLP):** Analyzes user reviews to categorize them as positive or negative.
* **Serialization:** The sentiment model is saved as a `.pkl` file using **Pickle**, allowing the system to analyze reviews without retraining.

### 3. Web Interface
* **Frontend:** Built with HTML/CSS and JavaScript (`content.js`) for a dynamic user experience.
* **Backend:** Integration via Python to serve recommendations and sentiment results.

---

## 🚀 Technologies Used
* **Python 3.x**
* **NLTK & Scikit-Learn** (NLP and Machine Learning)
* **Pandas & NumPy** (Data manipulation)
* **Flask/Heroku** (Deployment support via `Procfile`)
* **JavaScript & HTML5** (Web interface)

---

## 📈 Key Features
* **Real-time Suggestions:** Instant movie recommendations based on user input.
* **Review Analysis:** Automatically detects the tone of movie reviews to help users decide what to watch.
* **End-to-End Pipeline:** Covers everything from raw data preprocessing to a functional web UI.

---

## 🔗 Author
* **Ayushi Jain**
* **GitHub:** [Ayushi22jain](https://github.com/Ayushi22jain)
