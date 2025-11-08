BERT-Based Terrorism Tweet Detection
Overview

This project aims to detect terrorism-related content in tweets using Bidirectional Encoder Representations from Transformers (BERT). The model classifies tweets into categories such as Safe Text, Offensive, and Supports Terrorism by leveraging BERT’s contextual embeddings for semantic understanding.

The system is designed to assist in identifying and filtering online content that promotes or supports terrorism, improving the efficiency of social media monitoring and digital forensics.

Objectives

Develop a deep learning model capable of classifying tweets related to terrorism.

Utilize the BERT model for contextual understanding of textual data.

Achieve high classification accuracy compared to traditional NLP methods.

Contribute to the detection of extremist or harmful content online.

Dataset

Source: Custom dataset collected from Twitter (saved as terrorism.json).

Classes:

safe text

offensive

supports terrorism

Data Preprocessing Steps:

Removal of URLs, mentions, hashtags, and emojis.

Conversion of text to lowercase.

Cleaning of punctuation and special characters.

Tokenization using the BERT tokenizer.

Methodology
1. Data Preprocessing

Text normalization and cleaning.

Label encoding for the target variable.

Splitting into training, validation, and testing sets.

2. Model Architecture

Base Model: bert-base-uncased from Hugging Face Transformers.

A dropout layer followed by a dense output layer for classification.

Fine-tuning of BERT weights for domain-specific adaptation.

3. Training Configuration

Optimizer: AdamW

Loss Function: Categorical Cross-Entropy

Batch Size: 16

Epochs: 3–5

Evaluation Metrics: Accuracy, Precision, Recall, F1-score

4. Evaluation

Performance was evaluated using standard classification metrics, and confusion matrices were generated to visualize the model’s performance across different classes.

