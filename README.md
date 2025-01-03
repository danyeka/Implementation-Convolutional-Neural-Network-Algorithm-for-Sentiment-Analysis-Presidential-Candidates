## Implementation-Convolutional-Neural-Network-Algorithm-for-Sentiment-Analysis-Presidential-Candidates


**This repository contains the implementation and resources for a sentiment analysis project focused on comments about the 2024 Presidential and Vice-Presidential candidates on the Mata Najwa YouTube channel. The analysis was conducted using a Convolutional Neural Network (CNN) to classify comments into three sentiment categories: positive, negative, and neutral.**

# Table of Contents

1. Introduction
2. Dataset
3. Methodology
4. Model Performance
5. Usage
6. Acknowledgments

# Introduction
In this project, we analyzed 45,736 comments collected from the YouTube video titled "3 Bacapres Bicara Gagasan" from the Mata Najwa channel. This research leverages CNN, which achieves high accuracy in text-based sentiment classification by utilizing word embeddings and an optimized architecture. The model achieved an overall accuracy of 91%, demonstrating its effectiveness in processing and classifying social media sentiments.

# Dataset
 **The dataset includes:**

Source: Comments from the Mata Najwa YouTube channel.
Size: 45,736 comments.
Categories:
- Positive (4,228 comments)
- Neutral (9,047 comments)
- Negative (4,553 comments)

# Preprocessing Steps

- Cleansing: Removed irrelevant characters (hashtags, emoticons, etc.).
- Case Folding: Converted text to lowercase.
- Tokenization: Split sentences into words.
- Normalization: Converted informal words to formal equivalents.
- Stopwords Removal: Removed common words with low significance.
- Stemming: Reduced words to their root forms.

# Methodology
**Model Architecture**
**The CNN model consists of:**

- Embedding Layer: Converts text into numerical vectors.
- Convolutional Layer (Conv1D): Extracts features from the input vectors.
- Pooling Layer: Reduces dimensionality while preserving essential features.
- Fully Connected Layer: Classifies sentiments into three categories.

# Training and Testing

- Data split into 80% for training and 20% for testing.
- Oversampling was applied to balance class distribution using SMOTE.
- Evaluation Metrics
- Accuracy: 91%
- Precision, Recall, and F1-Score evaluated for all sentiment categories.

# Evaluation Metrics

Accuracy: 91%
Precision, Recall, and F1-Score evaluated for all sentiment categories.

# Model Performance
**Results**

- Training Accuracy: **90%**
- Validation Accuracy: **91%**
- Loss: **0.2593**

Example Predictions
| Comments                               | Predicted Sentiment  | Confidence Level | 
| ---------------------------------------| ---------------------| ---------------- |
| "Pembangunan saat ini semakin bagus"   | Positive             | 99.99%           | 
| "Berantas koruptor hukum mati"         | Negative             | 100.00%          |
| "Indonesia butuh pimpin jujur berani   | Neutral              | 62.54%           | 


## Acknowledgments

**This research was supported by the Informatics Department at Universitas Teknokrat Indonesia.** 
**Special thanks to the Mata Najwa channel for providing the dataset.**