# 🧠 Sentiment Analysis with Neural Networks

![Python](https://img.shields.io/badge/Python-3.11%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.10%2B-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)

A comprehensive Deep Learning NLP project that classifies text reviews into five distinct sentiment categories. This repository demonstrates the implementation and comparison of various neural network architectures, ranging from simple Dense networks to Transformers.

---

## 📖 Project Overview

Understanding user sentiment is critical for data-driven decision-making. This project builds an end-to-end Natural Language Processing (NLP) pipeline to predict sentiment on a 5-point scale:
1.  **Very Bad**
2.  **Bad**
3.  **Good**
4.  **Very Good**
5.  **Excellent**

The project addresses challenges such as **class imbalance**, **text preprocessing**, and **model optimization** using TensorFlow/Keras.

### Key Features
* **Advanced Preprocessing:** Custom pipeline including contraction expansion, emoji handling, stopword removal, and stemming.
* **Vectorization:** Utilizes TensorFlow's `TextVectorization` layer for end-to-end deployment capability.
* **Model Comparison:** Implements and benchmarks 5 different architectures (Dense, CNN, RNN, LSTM, Transformer).
* **Imbalance Handling:** Uses Class Weighting to ensure fair learning across minority classes.

---

## 📂 Repository Structure

```text
NN-Project-Repo/
├── data/                   # Dataset files (ignored by Git)
│   ├── train.csv           # Training data
│   └── test.csv            # Testing data
├── models/                 # Saved model artifacts (ignored by Git)
│   └── tensorflow_model/   # SavedModel format for deployment
├── notebooks/              # Experimentation & Testing
│   ├── sentimental_analysis_neural_network_project.ipynb  # Main training pipeline
│   └── test_script.ipynb   # Inference script for new data
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
