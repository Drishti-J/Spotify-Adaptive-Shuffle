# Spotify Adaptive Shuffle 🎧

A smart and intuitive song recommendation system that adapts to your listening behavior — built using the `spotify-dataset-1921-2020-160k-tracks` dataset.

---

## 🔍 Objective

To solve the frustration of bad shuffle experiences on music apps by using **user behavior (play/skip)** to generate personalized song recommendations.  
When a user skips multiple tracks in shuffle mode, this system **learns what they like and dislike** and adjusts future suggestions accordingly.

---

## ⚙️ How It Works

### 🔄 Adaptive Logic:
- If fewer than 10 songs are played, use **all played** songs to compute preferences.
- If 10 or more songs are played, use only the **last 10 played** songs (simulating a current session).
- Averages the features of these songs (valence, energy, acousticness, etc.).
- Compares the average vector to all **unseen songs** using cosine similarity.
- Recommends **Top 5 most similar songs** that haven’t been played or skipped yet.

### ❌ Skipped Song Penalty:
- Skipped songs are **excluded from future recommendations**.
- Helps avoid recommending songs similar to the ones the user dislikes.

---

## 📊 Accuracy Measurement

A custom **Feature-Based Accuracy Score** is used:
- Measures how close the recommended songs are to the **played profile** based on audio features.
- Output: Cosine similarity scores and a final accuracy percentage.
- Achieved **~99% accuracy** in most test runs.

---

## 🧪 Test Mode

Manually simulate a session:
- Pick specific songs as "played" and "skipped"
- Run the system and see recommendations
- Visually compare features and accuracy using graphs

---

## ✅ Output Sample

```
Song 1 similarity to played profile: 0.9936
Song 2 similarity to played profile: 0.9930
Song 3 similarity to played profile: 0.9923
Song 4 similarity to played profile: 0.9921
Song 5 similarity to played profile: 0.9920

✅ Feature-Based Accuracy Score: 99.26%
```

---

## 🗂️ Dataset Used

- Source: [Kaggle: spotify-dataset-1921-2020-160k-tracks](https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-1921-2020-160k-tracks)
- Cleaned for duplicates using `name + artist` logic

---

## 🚀 Future Ideas

- Integrate with Streamlit for interactive UI
- Add mood or genre-based filtering
- Penalize songs closer to skipped profile

---

## 📁 File Structure

- `Spotify_Adaptive_Shuffle_.ipynb`: Main notebook
- `spotify_adaptive_shuffle_.py`: Python script version
- `README.md`: You’re reading it 😉

---

## 🙋‍♀️ Author

**Drishti Jaiswal**  
“Music should adjust to you — not the other way around.”

---
