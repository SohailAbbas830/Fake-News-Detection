Fake News Detection using BERT and Hugging Face Transformers

## Project Overview

Fake news and misinformation have become major challenges in today's digital world. Social media platforms and online news sources spread information rapidly, making it difficult to distinguish between authentic and misleading content.

This project develops a Fake News Detection System using Natural Language Processing (NLP) and Transformer-based Deep Learning models. The model classifies news articles into two categories:

* **Real News (1)**
* **Fake News (0)**

The system is built using the Hugging Face Transformers library and a pre-trained BERT model, which is fine-tuned on a labeled fake news dataset.

---

##  Objectives

* Detect whether a news article is real or fake.
* Learn NLP preprocessing techniques.
* Apply transfer learning using BERT.
* Fine-tune transformer models for text classification.
* Evaluate model performance using standard classification metrics.

---

##  Dataset

Dataset: Kaggle Fake News Dataset

The dataset contains news articles labeled as:

| Label | Meaning   |
| ----- | --------- |
| 0     | Fake News |
| 1     | Real News |

### Dataset Features

* News Title
* News Content
* Label

---

## 🛠 Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Scikit-learn
* PyTorch
* Hugging Face Transformers
* Datasets
* Accelerate

### Deep Learning Framework

* PyTorch

### Model

* BERT (bert-base-uncased)

---

##  Project Workflow

### 1. Data Collection

Load fake and real news datasets from Kaggle.

### 2. Data Preprocessing

* Remove missing values
* Merge title and article text
* Create labels
* Shuffle dataset

### 3. Train-Test Split

* 80% Training Data
* 20% Testing Data

### 4. Tokenization

Convert text into BERT tokens using Hugging Face Tokenizer.

### 5. Model Fine-Tuning

Fine-tune a pre-trained BERT model for binary classification.

### 6. Evaluation

Evaluate performance using:

* Accuracy
* Precision
* Recall
* F1 Score

### 7. Prediction

Classify unseen news articles as Real or Fake.

---

##  Why BERT?

BERT (Bidirectional Encoder Representations from Transformers) is a Transformer-based language model that understands context from both directions of a sentence.

Advantages:

* Context-aware understanding
* State-of-the-art NLP performance
* Transfer learning capability
* Strong text classification performance

---

##  Model Architecture

Input Text
↓
BERT Tokenizer
↓
Input IDs + Attention Masks
↓
BERT Encoder
↓
Classification Layer
↓
Real / Fake Prediction

---

##  Training Configuration

| Parameter     | Value             |
| ------------- | ----------------- |
| Model         | bert-base-uncased |
| Learning Rate | 2e-5              |
| Batch Size    | 16                |
| Epochs        | 3                 |
| Optimizer     | AdamW             |
| Framework     | PyTorch           |
| GPU           | Kaggle Tesla T4   |

---

##  Results

The fine-tuned BERT model achieved strong performance on the test dataset.

Metrics used:

* Accuracy
* Precision
* Recall
* F1 Score

The model successfully learned semantic patterns within news articles and demonstrated high effectiveness in distinguishing real news from fake news.

---

##  Project Structure

text
Fake-News-Detection/
│
├── data/
│   ├── Fake.csv
│   └── True.csv
│
├── notebooks/
│   └── fake_news_detection.ipynb
│
├── fake_news_model/
│
├── results/
│
├── requirements.txt
│
├── README.md
│
└── .gitignore
```

---

##  Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Fake-News-Detection.git
```

Move into the project directory:

```bash
cd Fake-News-Detection
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

##  Run the Project

Open Jupyter Notebook:

```bash
jupyter notebook
```

Run:

```bash
fake_news_detection.ipynb
```

---

## 🔍 Example Prediction

Input:

```text
Government announces a new national education policy for universities.
```

Output:

```text
Real News
```

---

##  Concepts Learned

* Natural Language Processing (NLP)
* Text Preprocessing
* Tokenization
* Transformer Architecture
* BERT
* Transfer Learning
* Fine-Tuning
* Text Classification
* Model Evaluation
* Hugging Face Transformers

---

##  Academic Value

This project was developed as part of practical learning in:

* Artificial Intelligence
* Deep Learning
* Natural Language Processing
* Generative AI Foundations
* Transformer-Based Models

---

##  Future Improvements

* RoBERTa Implementation
* DistilBERT Optimization
* Multilingual Fake News Detection
* Real-Time News Verification API
* Streamlit Web Application
* Explainable AI Dashboard

---

##  Author

Sohail Abbas

BS Software Engineering

Islamia College University Peshawar

Interested in Artificial Intelligence, Data Science, Deep Learning, Generative AI, MLOps, and Cloud Data Engineering.

---

## If you found this project useful, consider giving the repository a star.

