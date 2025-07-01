# 🎧 Spotify Song Popularity Prediction

## 📌 Project Overview
This project focuses on **predicting the popularity of Spotify songs** based on various musical attributes using multiple machine learning models.  
The goal is to identify key features that may influence a song's popularity and develop predictive insights that can help artists, producers, and the music industry.

---

## 🎯 Problem Statement
In the highly competitive music streaming landscape, understanding **what makes a song popular** is essential.  
This project explores whether song attributes like acousticness, danceability, energy, and instrumentalness can help predict a song's Spotify popularity.

---

## 📚 Dataset
- **Source:** [Kaggle - Spotify Songs Dataset](https://www.kaggle.com/datasets/edalrami/19000-spotify-songs)
- **Size:** 18,835 songs | 15 features

Key attributes include:
- **Acousticness**
- **Danceability**
- **Energy**
- **Instrumentalness**
- **Loudness**
- **Speechiness**
- **Tempo**
- **Valence**
- **Song Popularity (Target Variable)**

---

## ⚙️ Methods & Workflow
1. **Data Cleaning:**  
   - Removed duplicates  
   - Validated data ranges  
   - Handled skewed distributions with log transformations

2. **Exploratory Data Analysis (EDA):**  
   - Correlation heatmaps  
   - Distribution plots  
   - Scatter plots  

3. **Statistical Testing:**  
   - Shapiro-Wilk test for normality  
   - QQ-Plots

4. **Feature Selection:**  
   - Removed insignificant features based on p-values from regression analysis

5. **Modeling Techniques Explored:**  
   - Naive Model (Baseline)  
   - Linear Regression  
   - Decision Trees  
   - K-Nearest Neighbors (KNN)  
   - Random Forest Regressor  
   - Gradient Boosting  
   - XGBoost

6. **Performance Metrics:**  
   - Root Mean Squared Error (RMSE)  
   - R-squared (R² Score)

---

## 🏆 Key Results
- ✅ **Best Model:** Random Forest Regressor  
- ✅ **Random Forest Performance:**  
   - Validation R²: ~0.365  
   - RMSE: 17.739  

- ✅ **Insights:**
   - No strong linear correlation between song attributes and popularity
   - Song duration, key, audio mode, and speechiness were insignificant predictors
   - Non-linear models performed better than linear ones

