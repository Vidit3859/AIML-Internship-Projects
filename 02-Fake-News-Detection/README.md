# 📰 Fake News Detection App

An NLP-based Machine Learning project that classifies news articles as **Fake** or **Real** using TF-IDF and Logistic Regression, with model explainability using top influencing words.

---

## 🚀 Live Demo

The application is deployed on Streamlit Cloud.
  
🔗 [Click here to try the Live App](https://news-article-classification-ml.streamlit.app/)

You can test the model by entering any news article text and instantly receive:
- Prediction (Fake / Real)
- Confidence Score
- Top Influential Words
- Model Explanation

---

## 📌 Project Overview

This project builds a binary text classification system that detects whether a news article is **Fake** or **Real**.

The model is trained using TF-IDF vectorization and Logistic Regression, achieving **98.75% accuracy** on the test dataset.

The app also provides:
- ✅ Prediction result
- 📊 Confidence score
- 🔍 Top influencing words
- 📖 Explanation of classification

---

## 🛠️ Tech Stack

- Python
- Scikit-learn
- Pandas
- NLTK
- Streamlit
- Pickle (Model Saving)

---

## 📂 Dataset

Dataset used:
- Fake.csv
- True.csv

The dataset contains labeled real and fake news articles.

⚠️ Note:  
The dataset is not included in this repository due to GitHub file size limitations. It is used only for training the model.

---

## ⚙️ Project Workflow

### 1️⃣ Data Collection
- Collected labeled dataset from Kaggle.

### 2️⃣ Text Preprocessing
- Lowercasing
- Removing punctuation
- Removing stopwords (NLTK)
- Stemming

### 3️⃣ Feature Extraction
- TF-IDF Vectorization

### 4️⃣ Model Training
- Logistic Regression classifier

### 5️⃣ Model Evaluation
- Accuracy: **98.75%**
- Precision, Recall, F1-score evaluated using classification report

### 6️⃣ Model Saving
- `fake_news_model.pkl`
- `tfidf_vectorizer.pkl`

### 7️⃣ Streamlit App
- User enters news text
- Model predicts Fake or Real
- Displays:
  - Confidence score
  - Top influencing words
  - Explanation message

---

## 🧠 Explainability Feature

The app displays the top TF-IDF weighted words influencing the prediction.

Example:
```
reuter (impact score: 2.18)
said (impact score: 1.18)
monday (impact score: 0.59)
```

This makes the model more transparent and interpretable.

---

## 📊 Model Performance

| Metric | Score |
|--------|-------|
| Accuracy | 98.75% |
| Precision | 0.99 |
| Recall | 0.99 |
| F1-score | 0.99 |

---

## ⚠️ Important Note

This model learns dataset-specific linguistic patterns (e.g., Reuters-style formatting vs clickbait tone).

It is **not a universal fact-checking system**, but a pattern-based text classification model.

---

## 📁 Project Structure

```
news-article-classification/
│
├── app.py
├── fake_news_model.pkl
├── tfidf_vectorizer.pkl
├── News_Article_Classification.ipynb
└── README.md
```

---

## ▶️ How to Run Locally

### 1️⃣ Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/news-article-classification.git
cd news-article-classification
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run Streamlit App

```bash
streamlit run app.py
```

App will open at:
```
http://localhost:8501
```

---

## 📌 Future Improvements

- Add deep learning model (LSTM / BERT)
- Add model comparison
- Improve UI styling
- Deploy on cloud permanently

---

## 👨‍💻 Author

**Vidit Kumar**

AI & Machine Learning Enthusiast  
Passionate about NLP, Web Development, and AI Systems

---

⭐ If you found this project useful, feel free to star the repository!

---