# Sentiment Analysis using Neural Networks

A deep learning project for multi-class sentiment analysis of text reviews. The model classifies reviews into five sentiment categories: **Very bad**, **Bad**, **Good**, **Very good**, and **Excellent**.

## Project Structure

```
NN Project/
├── data/                  # Datasets (not tracked by Git)
│   ├── train.csv
│   ├── test.csv
│   ├── submission.csv
│   └── Test cases.xlsx
├── models/                # Trained models (not tracked by Git)
│   ├── tensorflow_model.keras
│   └── tensorflow_model/
├── notebooks/             # Jupyter notebooks
│   ├── sentimental_analysis_neural_network_project.ipynb
│   └── test_script.ipynb
├── .gitignore
├── requirements.txt
└── README.md
```

## Getting Started

### Prerequisites

- Python 3.11+
- pip

### Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd NN-Project
   ```

2. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Download NLTK data (required for text preprocessing):

   ```python
   import nltk
   nltk.download('stopwords')
   nltk.download('punkt')
   nltk.download('punkt_tab')
   ```

4. Place your dataset files (`train.csv`, `test.csv`, etc.) in the `data/` directory.

### Running the Notebooks

1. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

2. Open `notebooks/sentimental_analysis_neural_network_project.ipynb` to train and evaluate the models.

3. Open `notebooks/test_script.ipynb` to run test predictions using a pre-trained model.

## Models

The project explores and compares several neural network architectures for sentiment classification:

- **Single-Layer Model** — A simple embedding + dense layer baseline.
- **Multi-Layer Model** — A deeper network with hidden layers and dropout.
- **CNN** — Convolutional neural network for text classification.
- **RNN (LSTM)** — Recurrent neural network using LSTM cells.
- **Transformer** — A custom Transformer encoder with multi-head self-attention.

## Tech Stack

- **TensorFlow / Keras** — Deep learning framework
- **NLTK** — Natural language preprocessing
- **Pandas & NumPy** — Data manipulation
- **Scikit-learn** — Evaluation metrics and utilities
- **Matplotlib** — Visualization
