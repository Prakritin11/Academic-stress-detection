# Academic-stress-detection

# Project Overview
This project presents a deep learning–based approach for academic stress level classification using self-reflective student texts. The system applies Long Short-Term Memory (LSTM) and Bidirectional LSTM (Bi-LSTM) architectures to identify stress levels as Low, Moderate, or High based on linguistic and contextual cues.

The project emphasizes ethical AI practices, originality through self-collected data, and explainable sequential modeling, making it suitable for educational and mental health applications.

# Objectives
- To design and implement an end-to-end deep learning pipeline for stress classification
- To analyze and compare the performance of LSTM vs Bi-LSTM architectures
- To evaluate model effectiveness using standard classification metrics
- To maintain a reproducible, well-documented academic codebase

# Dataset Description
- Source: Self-generated reflective academic texts
- Samples: ~300 short reflections
- Text Length: 1–4 sentences
- Stress Levels:
  - Low – Calm, positive, controlled emotions
  - Moderate – Mild anxiety and pressure
  - High – Overwhelming stress and difficulty coping
- Ethics:
  - No personal or sensitive data used
  - Labels assigned based on linguistic and contextual evidence
 
# Methodology
- Text Preprocessing
  - Tokenization
  - Vocabulary creation
  - Padding sequences to fixed length
- Embedding Layer
  - Trainable word embeddings learned from scratch
- Model Architectures
  - LSTM for sequential dependency learning
  - Bi-LSTM for bidirectional contextual understanding
- Classification
  - Fully connected dense layer
  - Softmax activation for multi-class prediction
 
# Training Details
Framework: PyTorch
Environment: Google Colab
Loss Function: Cross-Entropy Loss
Optimizer: Adam
Evaluation Metrics:
  - Accuracy
  - Precision
  - Recall
  - F1-score
