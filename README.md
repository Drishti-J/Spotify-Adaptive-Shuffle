
# 🎧 Adaptive Shuffle – A Smarter Spotify Recommendation Engine

Are you tired of Spotify's shuffle mode ignoring your mood?  
This project introduces **Adaptive Shuffle** — a feature-based, session-aware music recommendation engine that learns from your **played and skipped songs**.

---

## 💡 Why I Built This

I noticed that Spotify's shuffle mode didn't adapt when I skipped multiple songs — it just kept playing random tracks. So I built a system that actually learns from what I skip and what I vibe with — in real time.

---

## 🧠 What This System Does

- ✅ Learns from the **features of the songs you play**
- ❌ Avoids the **traits of skipped songs**
- 🎯 Recommends top 5 similar tracks using **cosine similarity**
- 📊 Evaluates predictions using **feature-based accuracy**
- 🧪 Visualizes how well recommendations match your taste

---

## 🔬 Dataset Used

- [Spotify Dataset 1921-2020 (160k tracks)](https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-1921-2020-160k-tracks)
- Contains audio features like valence, danceability, energy, acousticness, etc.

---

## 🚀 Key Features

- Feature-based recommendation using `valence`, `energy`, `tempo`, etc.
- Adaptive logic: focuses on the **last 10 played** songs
- (Optional) Skipped song penalty to sharpen accuracy
- Accuracy scoring via **cosine similarity** between played and recommended tracks

---

## 📊 Sample Output

![Screenshot 2025-04-09 at 1 07 24 PM](https://github.com/user-attachments/assets/2fbd9e7f-64c4-4aa5-ab98-079acbf5455e)
![Screenshot 2025-04-09 at 1 08 27 PM](https://github.com/user-attachments/assets/06c97b2e-9f9c-4c31-a3ee-a10701b59b04)
![Screenshot 2025-04-09 at 1 08 42 PM](https://github.com/user-attachments/assets/2404384c-d24a-4b2a-bb14-58470a81a17b)

---

## 🛠️ Tools & Tech

- Python, Pandas, NumPy
- Scikit-learn (cosine similarity, MinMaxScaler)
- Matplotlib for feature comparison

---

## 👩‍💻 Author

**Drishti Jaiswal**

---

## 📬 Feedback & Contributions

Open to ideas! Feel free to fork or suggest improvements.
