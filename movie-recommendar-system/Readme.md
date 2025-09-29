# 1. movie recommendar system
## 🎬 Movie Recommendation System

This is a **content-based movie recommendation system** built with **Python, Streamlit, and Machine Learning**.
It suggests movies similar to the one selected by the user, using **cosine similarity on movie features (tags, genres, keywords, cast, crew)**.

### 🚀 Features

* Interactive **Streamlit web app**
* Recommends **top 5 similar movies** based on your selection
* Fetches **movie posters from TMDB API** (with local caching for offline use)
* **Fallback placeholder poster** if API is unreachable
* Simple, lightweight, and easy to deploy

### 🛠️ Tech Stack

* **Python**
* **Pandas / Numpy** (data handling)
* **Scikit-learn** (cosine similarity)
* **Streamlit** (web interface)
* **Requests** (API calls)
* **Pickle** (model & data storage)

### 📂 Project Structure

```
movie-recommendar-system/
│── app.py                 # Main Streamlit app
│── movie_dict.pkl         # Movie metadata
│── similarity.pkl         # Precomputed similarity matrix
│── posters/               # Cached movie posters + placeholder
│── requirements.txt       # Dependencies
│── README.md              # Project documentation
```

### ▶️ How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/movie-recommender-system.git
   cd movie-recommender-system
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Run the Streamlit app:

   ```bash
   streamlit run app.py
   ```
4. Open the app in your browser → `http://localhost:8501`

### 🔑 API Key
This project uses **TMDB API** to fetch posters. You need to:

* Create a free account on [TMDB](https://www.themoviedb.org/)
* Get your API key
* Replace it in `app.py`

### 📌 Future Improvements

* Hybrid recommendations (content + collaborative filtering)
