# 📰 Fake News Detection Web App

This repository contains a machine learning-powered web application that detects whether a news article is **Fake** or **Real**. The application is built using **Python** and **Streamlit**, and it uses a **Logistic Regression** model trained on labeled news data.

---

## 📁 Repository Structure

.
├── app.py # Streamlit web application script
├── lr_model.jb # Pre-trained Logistic Regression model (joblib format)
├── vectorizer.jb # TF-IDF Vectorizer used to transform text data
├── requirements.txt # List of Python dependencies
├── Datasets/
│ ├── fake.csv # Dataset containing fake news articles
│ └── true.csv # Dataset containing real news articles
└── README.md # Project documentation

---

## 🧠 Overview

The goal of this application is to identify fake news articles using Natural Language Processing (NLP) and machine learning. The system takes input text from the user and predicts whether the news is fake or real using a trained Logistic Regression model.

- **TF-IDF Vectorization**: Text data is transformed using a TF-IDF (Term Frequency–Inverse Document Frequency) vectorizer to convert words into meaningful numerical representations.
- **Model Prediction**: A Logistic Regression model is used to make the final prediction.
- **User Interface**: A clean and responsive web interface is created using Streamlit to allow users to test the model in real time.

---

## 🧪 Datasets

The training data consists of two CSV files located in the `Datasets/` folder:

- `true.csv` – Contains real news articles.
- `fake.csv` – Contains fake news articles.

These datasets are used to train both the TF-IDF vectorizer and the classification model.

---

## 🧰 Model Files

- `lr_model.jb`: A trained Logistic Regression model saved using `joblib`. It is responsible for predicting the label of the input news.
- `vectorizer.jb`: A fitted TF-IDF vectorizer used to preprocess the input text and convert it into numerical features suitable for the model.

Both files are loaded inside the `app.py` script for real-time predictions.

---

## 💻 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/fake-news-detection.git
cd fake-news-detection
```


### 2. Create and Activate a Virtual Environment (Optional)

```bash
python -m venv venv
source venv/bin/activate         # On Windows use: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🚀 Run the Application

Use the command below to start the web app:

```bash
streamlit run app.py
```

This will launch a local Streamlit server and open the application in your default web browser.

---

## 🌐 About Streamlit

[Streamlit](https://streamlit.io/) is an open-source Python library that makes it easy to build custom web apps for machine learning and data science projects. It allows developers to turn Python scripts into interactive web apps with minimal effort.

In this project, Streamlit is used to create a user interface where users can input news content and receive instant predictions from the model.

---

## ✨ Features

- Clean and interactive user interface using Streamlit
- Real-time fake/real news prediction
- Lightweight and easy to deploy
- Built with open-source tools (Python, Scikit-learn, Streamlit)

---

## 📄 License

This project is licensed under the MIT License. You are free to use, modify, and share this software with proper attribution.

---

## 🙋‍♂️ Contact

For questions, suggestions, or contributions, feel free to open an issue or contact the maintainer via GitHub.

