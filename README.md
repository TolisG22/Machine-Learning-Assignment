# Machine Learning Assignment

This repository contains the complete implementation of the assignment for the **"Machine Learning"** course. The analysis is divided into three core sections (Sections A, B, and C), combining Descriptive Analytics with Predictive Analytics to strategically design and optimize an international advertising campaign.

## 📋 Project Structure & Key Results

### Section A: Descriptive Analytics & Seasonality
* **Seasonality Analysis:** A strong fluctuation in sales was identified, with November emerging as the absolute peak month ($2,118,885.67), followed by October and May. This trend highlights the necessity for a pre-promotion (Teasing Phase) starting as early as the beginning of autumn.
* **Fiscal Year 2005 Evaluation:** It was discovered that the apparent drop in 2005 sales was due to an incomplete dataset (records only available for months 1-5). A Like-for-Like comparison of the first five months revealed that 2005 was actually a year of organic growth.
* **Declining Category Analysis:** A significant revenue drop (-$1,089,683.81) was detected in the top-performing category **"Classic Cars"**, making it the primary repositioning target for the new marketing campaign.
* **Feature Correlation (Correlation Heatmap):** A strong positive correlation was confirmed between total sales (`SALES`) and premium pricing metrics, namely `PRICEEACH` (0.66) and `MSRP` (0.64), indicating that the target audience responds exceptionally well to high-value products.

### Section B: Sales Forecasting (Multiple Linear Regression)
* **Data Preparation:** Data merging was performed across the `Sales`, `Features`, and `Stores` source files. The `MarkDown1-5` variables were entirely excluded from modeling due to an excessive percentage of missing values (nulls).
* **Modeling (Store 1):** The regression model yielded a Root Mean Squared Error (RMSE) of 25,277.17.
* **Coefficient Analysis:** The **`IsHoliday` (1312.79)** variable proved to be the strongest positive driver for weekly sales, dictating that ad spending should scale up immediately prior to official holidays.

### Section C: Consumer Behavior Prediction (Naïve Bayes Classifier)
* **User Profiling:** Exploratory data analysis indicated that heavy internet users tend to ignore digital advertisements (ad-fatigue), whereas older demographics exhibit higher overall ad-engagement.
* **Model Evaluation:** The Naïve Bayes classifier achieved an outstanding **Overall Accuracy of 94.50%** on the test set (200 users). 
* **Confusion Matrix Metrics:** The model recorded 106 True Positives, 83 True Negatives, 6 False Positives, and 5 False Negatives, maintaining stable Precision and Recall scores of 0.95 for the click class.
* **Business Application:** The model enables **real-time Micro-targeting**, serving ads exclusively to web visitors with a high probability of conversion, thereby minimizing ad-waste and maximizing ROI.

---

## 🛠️ Technologies & Python Libraries

The project was implemented using **Python 3.x** along with the following specialized libraries:
* `pandas` & `numpy` (Data cleaning, merging, and preprocessing)
* `matplotlib` & `seaborn` (Data visualization, Pair Plots, and Correlation Heatmaps)
* `scikit-learn` (Model training, evaluation of Linear Regression and Naïve Bayes, and generation of Confusion Matrices & Classification Reports)

---
