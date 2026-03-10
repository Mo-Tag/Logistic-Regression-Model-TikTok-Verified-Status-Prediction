# Logistic-Regression-Model-TikTok-Verified-Status-Prediction

## Introduction
Navigating the complexities of user verification on platforms like TikTok is key for content moderation and analysis. This project builds a logistic regression model in Python to predict a user's verified status based on video features, such as duration, view counts, and transcription text length. Using a real-world TikTok dataset, it covers exploratory data analysis (EDA), preprocessing (including handling class imbalance via upsampling), model construction, and evaluation to estimate the probability of verification—a binomial outcome.
The purpose is to demonstrate EDA and regression modeling skills, with the goal of creating an interpretable model that reveals how video characteristics relate to verified users, potentially informing broader claim vs. opinion prediction models.

<img width="940" height="818" alt="image" src="https://github.com/user-attachments/assets/3f3c1bf2-a074-48d7-b160-2c907034ef7f" />

## Skills Showcased 🛠️

### Data Manipulation and EDA:
Inspecting data, handling missing values, duplicates, outliers, and class imbalance with Pandas and NumPy.

### Data Visualization:
Generating boxplots, histograms, heatmaps, and confusion matrices using Matplotlib and Seaborn.

### Data Preprocessing:
One-hot encoding categoricals with scikit-learn, feature engineering (e.g., extracting transcription text length), and resampling for balance.

### Model Building:
Fitting logistic regression via scikit-learn with train-test splits and adjusted iterations for convergence.

### Model Evaluation:
Producing confusion matrices, classification reports, and coefficient interpretations for insights.


## Visualizations Utilized 📈

### Boxplots:
For outlier detection in features like video duration, views, likes, and comments.

### Histograms:
To compare distributions, such as transcription text lengths between verified and unverified users.

### Heatmaps:
Visualizing feature correlations to check for multicollinearity.

<img width="794" height="648" alt="image" src="https://github.com/user-attachments/assets/9fe63493-db27-4806-bb2b-d828a1bf4bcd" />

## Project Overview 🔎
Structured around the PACE framework (Plan, Analyze, Construct, Execute), this project starts with data loading and EDA to handle anomalies and verify assumptions like no multicollinearity. Key steps: Dropping missing values, capping outliers (e.g., in likes and comments), upsampling the minority verified class for balance, adding a text_length feature, and encoding categoricals. The logistic regression model uses features like video duration and counts, achieving 65% accuracy with strong recall (84%) for unverified users. Visuals ensure transparency, from correlation checks to final evaluations.
The dataset emphasizes video metrics and author status, targeting verified status prediction to aid TikTok's content prioritization.

<img width="940" height="394" alt="image" src="https://github.com/user-attachments/assets/cd14ec8d-aa82-417f-80cc-025bf1af78ee" />

## Conclusion
This project applies logistic regression to TikTok data, yielding a model with decent predictive power (65% accuracy, 84% recall for unverified). It reveals that longer videos boost verification odds slightly, while other features show minimal impact. By addressing multicollinearity (e.g., dropping like counts), the model remains reliable. These insights can guide TikTok in refining user verification strategies and integrating into claim/opinion models. A solid base for advanced techniques like feature selection or ensembles!
