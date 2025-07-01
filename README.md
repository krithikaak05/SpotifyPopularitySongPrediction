# 🎵 Spotify Song Popularity Prediction 🎵  
*A Machine Learning Exploration into What Makes a Song Go Viral*  

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white) 
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Modeling-orange?logo=Scikit-Learn&logoColor=white) 
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)  

---

## 🚀 Project Summary
This project aims to **predict the popularity of Spotify songs** based on their musical and technical attributes.  
Using **data science and machine learning**, we investigated whether it’s possible to estimate a song's popularity score using features like energy, danceability, and tempo.

> 🎯 **Goal:** Build predictive models to uncover patterns that make songs popular on Spotify.

---

## 📦 Table of Contents
- [🎯 Problem Statement](#-problem-statement)
- [📚 Dataset](#-dataset)
- [⚙️ Approach](#️-approach)
- [🛠️ Tools Used](#️-tools-used)
- [📊 Model Performance](#-model-performance)
- [💡 Key Takeaways](#-key-takeaways)
- [🗂️ Project Structure](#️-project-structure)
- [🚀 How to Run](#-how-to-run)
- [👩‍💻 Authors](#-authors)
- [📄 References](#-references)

---

## 🎯 Problem Statement
The popularity of songs on Spotify is influenced by various audio features, but **what exactly makes a song popular?**  
We set out to analyze and predict Spotify song popularity using:
- Song-specific attributes (acousticness, danceability, energy, etc.)
- Regression and ensemble machine learning models

---

## 📚 Dataset
- 📂 **Source:** [Kaggle: Spotify Songs Dataset](https://www.kaggle.com/datasets/edalrami/19000-spotify-songs)
- 📊 **Size:** 18,835 songs | 15 features
- 🎧 **Attributes:**
  - Acousticness
  - Danceability
  - Energy
  - Instrumentalness
  - Tempo
  - Valence
  - Loudness
  - Speechiness
  - Key, Mode, Duration, and more

---

## ⚙️ Approach
### 🔍 Exploratory Data Analysis (EDA)
- Visualized attribute distributions
- Investigated correlations and multicollinearity
- Performed log transformations to handle skewed data

### 🧹 Data Preprocessing
- Removed duplicates
- Handled skewness and outliers
- Standardized features

### 🧮 Model Development
- Baseline: Naive model
- Linear Regression
- Decision Trees
- K-Nearest Neighbors (KNN)
- Random Forest 🌟 (Best Performer)
- Gradient Boosting
- XGBoost

### 📐 Evaluation Metrics
- Root Mean Squared Error (RMSE)
- R-squared (R² Score)

---

## 🛠️ Tools Used
- **Python 3.8+**
- **Scikit-Learn**
- **Pandas & NumPy**
- **Matplotlib & Seaborn**
- **Spotify API (Reference)**

---

## 📊 Model Performance
| Model                | R² Score (Validation) | RMSE   | Notes                           |
|---------------------|------------------------|--------|---------------------------------|
| Naive Model          | -9.74                  | 22.17  | Baseline                       |
| Linear Regression    | 0.043                  | 21.62  | Poor fit, significant residuals |
| Decision Trees       | -0.14                  | 24.60  | Overfitting and underfitting    |
| KNN                  | -10.58                 | 21.39  | Very poor performance           |
| **Random Forest**    | **~0.365**             | 17.74  | ⭐ Best performing model ⭐      |
| Gradient Boosting    | ~0.191                 | 19.99  | Average                        |
| XGBoost              | ~0.240                 | 19.41  | Moderate                       |

---

## 💡 Key Takeaways
- 🎶 **No strong linear correlation** between most song features and popularity.
- 🏆 **Random Forest Regressor outperformed** other models despite low variance explanation (~36.5%).
- 🔎 Features like **song duration, key, mode, and speechiness were dropped** due to insignificant impact.
- 📉 The dataset was complex with **non-linear patterns** and low predictability using basic features alone.

---

## 🗂️ Project Structure
```plaintext
Spotify-Popularity-Prediction/
├── FinalCode_PT1.ipynb      # Full Google Colab Notebook
├── FinalCode_PT2.pdf      # Full Google Colab Notebook
├── README.md          # Project Overview (this file)
