# X Tweets Sentiment Analysis 🧠💬

This project performs sentiment analysis on a dataset of **1.6 million tweets** using **Machine Learning** and **NLTK**. It uses a **Logistic Regression** model to classify tweets as having positive or negative sentiment.

---

## 📊 Dataset

- **Name:** [Sentiment140](https://www.kaggle.com/datasets/kazanova/sentiment140)  
- **Source:** Kaggle  
- **Size:** 1.6 million labeled tweets  
- **Labels:**
  - `0`: Negative
  - `4`: Positive → converted to `1`

---

## 🚀 Project Workflow

### 1. Load Data
- Dataset downloaded from Kaggle.
- Loaded using pandas into a DataFrame.

### 2. Preprocessing
- Renamed columns for clarity.
- Converted sentiment labels: `4 → 1`.
- Defined custom text cleaning function:
  - Lowercasing
  - Removing punctuation
  - Removing stopwords
  - Applying stemming using `PorterStemmer`
- Created new column: `stemmed_content`.

### 3. Vectorization
- Used `TfidfVectorizer` to convert cleaned text to numerical format.

### 4. Data Split
- Split into training and testing sets using `train_test_split`.

### 5. Model Training
- Applied **Logistic Regression** (supervised learning).
- Trained on TF-IDF features.

### 6. Evaluation
- Accuracy on test data: **77.716%**

### 7. Model Persistence
- Model saved using `pickle` as `model.pkl`.
- Reloaded model for prediction demo.

### 8. Prediction
- Performed sentiment predictions on sample tweets.

---

## 🛠️ Tech Stack

- Python
- Pandas, Numpy
- NLTK
- Scikit-learn
- TfidfVectorizer
- Pickle
- Jupyter Notebook

---

## 📂 Project Structure

X-Tweets-Sentiment-Analysis/
│
├── sentiment_analysis.ipynb # Jupyter notebook with full ML pipeline
├── model.pkl # Saved logistic regression model
├── requirements.txt # Python dependencies
└── README.md # Project overview

##📬 Contact
Author: Rohit Mishra
📧 Email: rohitmishra5560@gmail.com
🔗 LinkedIn: [](https://www.linkedin.com/in/rohit-mishra-93s5b/)

