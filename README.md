# 🎵 Spotify Adaptive Shuffle

A personalized, feature-based song recommendation engine that mimics how an ideal shuffle mode *should* work — adapting in real-time based on the user’s skip and play behavior.

---

## 👩‍💻 Created By
**Drishti Jaiswal**

---

## 🧠 Concept

Spotify's shuffle often feels random. What if it *learned* your preferences from what you skipped or played?

This project builds a smart shuffle using real **audio features** (like energy, valence, danceability) to:
- Track user behavior during listening sessions.
- Recommend songs that **closely match** previously played tracks.
- Avoid songs that are similar to skipped tracks.

---

## 📊 Dataset

Used: [`spotify-dataset-1921-2020-160k-tracks`](https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-1921-2020-160k-tracks)

Includes over 170k songs and their acoustic features like:
- `energy`, `valence`, `tempo`, `speechiness`, etc.

---

## 🚀 Features

- ✅ Duplicate removal by name + artist
- ✅ Soft deduplication using audio features
- ✅ Vector averaging of played songs
- ✅ Cosine similarity to suggest songs
- ✅ Feature-based accuracy calculation
- ✅ Bar chart comparison for interpretability
- ✅ Random session simulation for realistic testing

---

## 🧪 How It Works

1. You play or skip a few songs.
2. The system builds an **audio profile** of your played songs.
3. Then, it recommends top `k` songs **most similar** to that profile.

---

## 📈 Accuracy Metric

The system evaluates the cosine similarity between:
- The average feature vector of played songs, and
- Each recommended song.

This gives a **Feature-Based Accuracy Score** showing how "on-point" the suggestions are.

---

## 🖥️ Run It Yourself

```bash
pip install pandas numpy scikit-learn matplotlib
```

Or use it in **Google Colab** — all code is Jupyter-ready!

---

## 📂 Files

- `Spotify_Adaptive_Shuffle_.ipynb` – Complete notebook with end-to-end logic
- `spotify_adaptive_shuffle.py` – Python script version (modularized)
- `README.md` – Project description and setup guide

---

## 📌 Future Scope

- Streamlit UI for song inputs & real-time feedback
- Integration with Spotify API for live testing
- Advanced skip-penalty scoring logic
- Clustering-based playlist generation

---

## ❤️ Special Thanks

To all the tracks we skipped, thanks for helping us learn.