# NLP with Disaster Tweets — Kaggle Competition

## Overview

This project is part of the **"Natural Language Processing with Disaster Tweets"** Kaggle competition, where the goal is to build a model that can accurately classify whether a tweet refers to a real disaster or not. This is a **binary classification problem** that applies Natural Language Processing (NLP) techniques to social media content.

The motivation behind this task is rooted in **emergency response**, where accurately identifying disaster-related tweets can significantly aid in real-time decision-making.

## Problem Domain

This task lies within **Natural Language Processing (NLP)**, a subfield of AI that enables machines to process and understand human language. We applied NLP methods to extract useful representations from tweet text and used those features to build deep learning models for classification.

## Model Development

The core of the project focused on deep learning using **LSTM (Long Short-Term Memory)** models. We explored various model architectures, including:

- **Model #1**: Base LSTM model with GloVe embeddings and dropout  
- **Model #2**: LSTM with modified dropout and learning rate  
- **Model #3**: Simplified model to reduce overfitting  
- **Model #4**: Stacked LSTM with L1 regularization  
- **Model #5**: Bidirectional LSTM for richer context learning  

Each model was evaluated using training/validation accuracy and submitted to Kaggle for public scoring.

### ✅ Final Model Selection

After evaluating both **validation accuracy** and **Kaggle public leaderboard scores**, we selected **Model #1** as our final model:

| Model | Kaggle Score | Notes |
|-------|--------------|-------|
| **#1** | **0.80202** | Best performing model, well-balanced |
| #2     | 0.79497      | Moderate dropout, good but slightly lower |
| #3     | 0.77750      | Least overfitting but lower performance |
| #4     | 0.79344      | Stacked LSTM + regularization, risk of overfitting |
| #5     | 0.80018      | Strong architecture (BiLSTM), close contender |

Model #1 delivered the best score and generalization, making it the optimal choice for submission. Model #5 is also a strong alternative.

