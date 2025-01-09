# Fake News Detector

## Overview

The Fake News Detector is a machine learning project designed to address the growing issue of misinformation by distinguishing between real and fake news articles.

This project was collaboratively developed by:
- **Aiesha Ayub**
- **Aidan Murphy**
- **Anna Nguyen**
- **Jialene Westcott**

## Dataset

The dataset for this project was sourced from [Kaggle](https://www.kaggle.com/datasets/bhavikjikadara/fake-news-detection/data). It includes two key files:
- `true.csv`: Contains verified real news articles.
- `fake.csv`: Contains articles classified as fake news.

These files were preprocessed and combined into a single dataset with over 44,000 rows for training, testing, and validation. Preprocessing steps included removing unnecessary characters, tokenization, and vectorization.

## Project Goals

The primary objectives of the project are:
1. Identify the most common sources of disinformation.
2. Detect linguistic patterns, keywords, and other markers characteristic of fake news.
3. Develop a user-friendly system for real-time fake news detection.

## Methods

The project employed the following models to classify news articles:
- **Transformers**: Language models for natural language understanding.
- **Multi-Layer Perceptron (MLP)**: A type of neural network for classification tasks.
- **Support Vector Machine (SVM)**: A model for binary classification in multi-dimensional spaces.
- **Naive Bayes**: A probabilistic classifier based on Bayes' Theorem.

### Ensemble Model

To enhance performance, an ensemble model was built by combining the outputs of the individual models. The ensemble approach leverages the strengths of each model to improve accuracy and reliability.

## Results

The following table summarizes the training accuracies of each model:

| Model Name      | Training Accuracy |
|-----------------|-------------------|
| Transformers    | 99.6%            |
| MLP             | 99.2%            |
| SVM             | 98.6%            |
| Naive Bayes     | 94.1%            |
| **Combined**    | **97.9%**        |

The ensemble model demonstrated improved robustness in detecting fake news compared to individual models.

## Features

### Graphical User Interface (GUI)
A GUI was developed to make the Fake News Detector accessible to non-technical users. The interface allows users to input text from an article, which the system analyzes to determine whether the article is real or fake. The GUI displays model scores alongside the final prediction.

### Insights
- Common patterns in fake news include repeated use of specific political terms, emotionally charged words, and exaggerated claims.
- Preprocessing and data cleaning significantly impacted the performance of all models.

## Limitations

While the model achieved high accuracy on the dataset, its effectiveness is limited to articles from 2016–2017. Expanding the dataset to include more recent articles would improve its applicability and robustness in detecting contemporary fake news.

## Future Work

Potential areas for improvement include:
1. Expanding the dataset to include a wider temporal and topical range.
2. Enhancing the model to handle multilingual content.
3. Increasing public awareness of disinformation through educational tools integrated with this system.

## Acknowledgments

Source:
- [Kaggle Dataset](https://www.kaggle.com/datasets/bhavikjikadara/fake-news-detection/data)
