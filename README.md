# 🤖 Machine Learning Course Project

> **Ho Chi Minh City University of Technology (HCMUT)**
> Faculty of Computer Science and Engineering
> Semester I – Academic Year 2025–2026

---

## 📋 Course Information

| Field | Details |
|-------|---------|
| **Course Name** | Machine Learning |
| **Instructor** | Dr. Truong Vinh Lan |
| **Contact** | lantv@hcmut.edu.vn |
| **Institution** | Ho Chi Minh City University of Technology – VNU-HCM |
| **Department** | Computer Science |
| **Semester** | Semester 252, Academic Year 2025–2026 |

---

## 👥 Team Information – Group 1

| No. | Full Name | Student ID | Role |
|-----|-----------|------------|------|
| 1 | Nguyen The Hoang | 2352354 | **Team Leader** |
| 2 | Ngo Tran Dinh Duy | 2352179 | Member |
| 3 | Nguyen Viet Nam | 2352780 | Member |
| 4 | Trinh Gia Hiep | 2352343 | Member |
| 5 | Tran Lam Bieu | 2352116 | Member |

---

## 🎯 Project Overview

This project implements end-to-end **traditional Machine Learning pipelines** across three different data modalities: tabular data, text data, and image data. The goal is to gain hands-on experience with each stage of the ML workflow — from raw data exploration to model evaluation — and to systematically compare the performance of different configurations and algorithms.

Each assignment follows the standard ML pipeline:

```
Raw Data → EDA → Preprocessing → Feature Extraction → Model Training → Evaluation & Comparison
```

All implementations are delivered as **Google Colab notebooks** that run end-to-end without errors via *Runtime → Run all*, with datasets downloaded automatically from public sources.

---

## 📂 Assignments

### Assignment 1 – Tabular Data

**Objective:** Build a configurable traditional ML pipeline for structured/tabular data.

**Dataset Requirements:**
- Must contain missing values (to practice imputation techniques)
- Must contain categorical features (to practice encoding techniques)
- Must be sufficiently large for meaningful results

**Pipeline Steps:**
1. **EDA** – Descriptive statistics, distribution analysis, correlation matrix, outlier detection, missing value visualization
2. **Preprocessing** – Missing value imputation (mean/median/mode/KNN), categorical encoding (one-hot, label encoding), feature scaling (MinMaxScaler, StandardScaler)
3. **Dimensionality Reduction** – PCA with configurable variance retention (90%, 95%, 99%)
4. **Model Training** – Logistic Regression, Support Vector Machine (SVM), Random Forest
5. **Evaluation** – Accuracy, Precision, Recall, F1-score, Confusion Matrix, cross-validation

**Key Comparisons:** Different scalers x Different PCA thresholds x Different classifiers

---

### Assignment 2 – Text Data

**Objective:** Build a text classification pipeline using both traditional and modern feature extraction methods.

**Dataset Requirements:**
- Diverse content (multiple topics or classification labels)
- Sufficiently large sample size

**Pipeline Steps:**
1. **EDA** – Word frequency analysis, text length distribution, label distribution, vocabulary statistics
2. **Preprocessing** – Tokenization, stopword removal, stemming/lemmatization, padding
3. **Feature Extraction:**
   - *Traditional:* Bag-of-Words (BoW), TF-IDF, n-gram
   - *Modern (Deep Learning Embeddings):* Word2Vec, GloVe, BERT / RoBERTa / DistilBERT
4. **Embedding Storage** – Save extracted embeddings as `.npy` or `.h5` files
5. **Model Training** – Naive Bayes, Logistic Regression, SVM (on traditional features); simple neural network or fine-tuning (on deep embeddings)
6. **Evaluation** – Accuracy, Precision, Recall, F1-score; comparison between traditional vs. modern approaches

---

### Assignment 3 – Image Data

**Objective:** Build an image classification pipeline leveraging pretrained deep learning models for feature extraction, combined with traditional classifiers.

**Dataset Requirements:**
- Sufficient number and diversity of images per class
- Compatible size for processing on Google Colab

**Pipeline Steps:**
1. **EDA** – Image size distribution, color channel analysis, class distribution, sample visualization
2. **Preprocessing** – Resizing, normalization, data augmentation (optional)
3. **Feature Extraction (Pretrained Models):**
   - CNN-based: VGG16, ResNet50, EfficientNet
   - Transformer-based: Vision Transformer (ViT), Swin Transformer
4. **Feature Storage** – Save extracted feature vectors as `.npy` or `.h5` files
5. **Model Training** – Logistic Regression, SVM, Random Forest (on extracted features)
6. **Evaluation** – Accuracy, F1-score; comparison across different pretrained backbones

---

## 🗂️ Repository Structure

```
ML-Assignment-2025/
│
├── notebooks/                   # Google Colab notebooks
│   ├── bai1_tabular.ipynb       # Assignment 1 – Tabular Data
│   ├── bai2_text.ipynb          # Assignment 2 – Text Data
│   └── bai3_image.ipynb         # Assignment 3 – Image Data
│
├── modules/                     # Reusable Python modules
│   ├── preprocessing.py         # Data cleaning, imputation, encoding, scaling
│   ├── feature_extraction.py    # Feature engineering and embedding extraction
│   ├── models.py                # Model wrappers and training utilities
│   └── evaluation.py            # Metrics, plots, and result comparison
│
├── reports/                     # Written reports
│   └── report_final.pdf         # Final PDF report
│
├── features/                    # Pre-extracted feature files
│   ├── bai2_tfidf.npy           # TF-IDF vectors – Assignment 2
│   ├── bai2_bert_embeddings.npy # BERT embeddings – Assignment 2
│   ├── bai3_vgg16_features.npy  # VGG16 features – Assignment 3
│   └── bai3_resnet_features.npy # ResNet features – Assignment 3
│
└── README.md
```

---

## Setup & Installation

### Prerequisites

- Python 3.8+
- Google Colab (recommended) or local environment with GPU support

### Install Dependencies

```bash
# Core ML libraries
pip install numpy pandas scikit-learn matplotlib seaborn

# Deep learning
pip install torch torchvision torchaudio
pip install tensorflow keras

# NLP
pip install transformers datasets
pip install nltk gensim

# Image processing
pip install Pillow opencv-python

# Utilities
pip install h5py tqdm
```

### Running the Notebooks

1. Open the desired notebook in **Google Colab**
2. Select **Runtime -> Run all**
3. The dataset will be **automatically downloaded** from a public source (link provided inside each notebook)
4. Do NOT mount personal Google Drive — all data is fetched directly into the Colab runtime

---

## 📊 Evaluation Criteria

| Criterion | Weight |
|-----------|--------|
| Complete traditional ML pipeline | 40% |
| Quality of analysis and experiments | 25% |
| Report clarity and structure | 20% |
| Product completeness (Colab runs without error, correct file structure) | 10% |
| Teamwork evidence | 5% |
| **Bonus:** Deep learning pipeline comparison | +5% |
| **Bonus:** GitHub with complete README | +5% |

---

## 🔗 Links

| Resource | Link |
|----------|------|
| Colab Notebook – Assignment 1 | *Coming soon* |
| Colab Notebook – Assignment 2 | *Coming soon* |
| Colab Notebook – Assignment 3 | *Coming soon* |
| Final Report (PDF) | *Coming soon* |

---

## 📅 Timeline

| Milestone | Date |
|-----------|------|
| Group registration deadline | 27/02/2026 |
| Progress Report #1 | 08/03/2026 |
| Progress Report #2 | 22/03/2026 |
| Progress Report #3 | 12/04/2026 |
| Progress Report #4 | 26/04/2026 |

---

## 📬 Submission

Final submission is via **Google Form** (link provided on LMS). Only **one upload** is allowed — ensure the `.zip` file is complete and correct before submitting.

The `.zip` file must follow this structure:
```
GroupX_StudentIDs.zip
├── notebooks/
├── modules/
├── reports/
└── features/
```

---

*Last updated: 08/03/2026*
