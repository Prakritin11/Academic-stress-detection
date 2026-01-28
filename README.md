# Academic-stress-detection

# Project Overview
This project presents a deep learning–based approach for academic stress level classification using self-reflective student texts. It applies Long Short-Term Memory (LSTM) and Bidirectional LSTM (Bi-LSTM) architectures to classify stress levels as Low, Moderate, or High based on linguistic and contextual cues.

The project emphasizes ethical AI practices, originality through self-generated reflective texts, and explainable sequential modeling, making it suitable for educational and mental health applications.

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
  - Preserves student privacy and allows scalable monitoring.
 
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
- Framework: PyTorch
- Environment: Google Colab (GPU)
- Optimizer: Adam (learning rate 0.001)
- Loss Function: Cross-Entropy Loss
- Batch Size: 16
- Epochs: 30
- Dataset Split: 70% train, 20% validation, 10% test

# Evaluation Metrics:
  - Accuracy
  - Precision
  - Recall
  - F1-score

# Results
- Both LSTM and Bi-LSTM achieved 100% accuracy, precision, recall, and F1-score on the synthetic dataset.
- Bi-LSTM demonstrated stronger contextual understanding due to bidirectional sequence modeling.
- Training and validation losses converged smoothly, showing stable and robust learning.
- Average inference time per sample:
  - LSTM: ~0.85 ms
  - Bi-LSTM: ~0.92 ms
 
# Conclusion and Future Work

- Deep learning models (LSTM/Bi-LSTM) effectively classify stress levels in synthetic reflective texts.
- The approach is ethical, scalable, non-invasive, and can be applied to educational or workplace stress monitoring.
- Future Enhancements:
  - Use real student datasets with larger vocabulary
  - Incorporate advanced architectures (attention mechanisms, transformers)
  - Enable real-time monitoring via integration with Learning Management Systems (LMS)
  - Explore multimodal inputs such as physiological or behavioral data
 
# Requirements
- torch==2.2.0
- torchvision==0.17.1
- torchaudio==2.2.0
- numpy==1.24.4
- pandas==2.1.1
- scikit-learn==1.3.0
- matplotlib==3.8.0
- seaborn==0.12.3
- jupyter==1.0.0
- notebook==7.2.3
- tqdm==4.66.1

