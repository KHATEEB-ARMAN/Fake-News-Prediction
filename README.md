﻿# Fake-News-Prediction
Overview

This project, completed in May 2025, aims to classify news articles as fake or true using machine learning techniques. It leverages natural language processing (NLP) to preprocess text data and a supervised learning model to predict the authenticity of news articles. The project uses a dataset of labeled news articles and achieves high accuracy in distinguishing between fake and true news.

Features

Data Preprocessing: Cleans and processes text data using tokenization, stop-word removal, and TF-IDF vectorization.

Model: Logistic Regression classifier (with options for other models like Random Forest or BERT).

Evaluation: Metrics include accuracy, precision, recall, and F1-score.

Dataset: Sourced from Kaggle's Fake News Dataset (or specify your dataset).

Tools: Python, scikit-learn, NLTK, Pandas, Jupyter Notebook.

Installation

Clone the repository:

git clone https://github.com/your-username/fake-true-news.git



Navigate to the project directory:

cd fake-true-news



Install dependencies:

pip install -r requirements.txt



Ensure Python 3.8+ is installed.

Usage





Prepare the Dataset:





Place the dataset (e.g., news.csv) in the data/ folder.



Update the dataset path in config.yaml if necessary.



Run the Preprocessing Script:

python preprocess.py

This cleans the text data and saves processed files in data/processed/.



Train the Model:

python train.py

Outputs a trained model saved as models/logistic_regression.pkl.



Evaluate the Model:

python evaluate.py

Generates a report with accuracy, precision, recall, and F1-score.



Predict on New Data:

python predict.py --input "path/to/new_article.txt"

Outputs whether the article is fake or true.

Project Structure

fake-true-news/
├── data/
│   ├── raw/                # Raw dataset
│   ├── processed/          # Processed dataset
├── models/                 # Trained models
├── notebooks/              # Jupyter notebooks for exploration
├── src/
│   ├── preprocess.py       # Text preprocessing script
│   ├── train.py            # Model training script
│   ├── evaluate.py         # Model evaluation script
│   ├── predict.py          # Inference script
├── requirements.txt        # Dependencies
├── config.yaml             # Configuration file
└── README.md               # Project documentation

Results





Achieved 85%+ accuracy on the test set using Logistic Regression.



Detailed evaluation metrics are available in reports/evaluation_report.txt.

Future Improvements





Incorporate deep learning models like BERT for better performance.



Add real-time data scraping from X or web sources for dynamic predictions.



Enhance feature engineering with sentiment analysis or source credibility.

Contributing

Feel free to open issues or submit pull requests. Contact [your-email@example.com] for collaboration.
