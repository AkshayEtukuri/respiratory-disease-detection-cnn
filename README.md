# 🛡️ Classification of Online Toxic Comments Using Machine Learning

A multi-label text classification system that detects and categorizes toxic online comments into six threat categories using six machine learning algorithms, with comparative performance analysis.

---

## 📌 Problem Statement

Toxic comments — abusive, disrespectful, or threatening language on social media — suppress healthy online discourse and drive users away from discussions. This project builds an automated system to classify comments as toxic or non-toxic, and further categorizes toxic content into specific labels to help platforms moderate content at scale.

---

## 🎯 Project Highlights

- **Multi-label classification** across 6 toxicity categories: `toxic`, `severe toxic`, `obscene`, `threat`, `insult`, `identity hate`
- **6 ML algorithms** trained and benchmarked on the same dataset
- **Best accuracy: 95% (SVM)** | **Best overall model: Logistic Regression** (89.46% accuracy, 2.43% hamming loss)
- **Random Forest** achieved 100% accuracy with 0% loss on training data
- End-to-end pipeline: data upload → preprocessing → vectorization → training → prediction

---

## 📊 Algorithm Performance Comparison

| Algorithm           | Accuracy  | Hamming Loss | Log Loss |
|---------------------|-----------|--------------|----------|
| Logistic Regression | **89.46%** | **2.43%**   | —        |
| SVM Classifier      | **95%**   | 0.05%        | —        |
| Random Forest       | 100%      | 0%           | Best     |
| Naïve Bayes         | —         | —            | —        |
| Decision Tree       | —         | —            | —        |
| KNN                 | —         | —            | —        |

> ✅ **Final model selected: Logistic Regression** — best balance of accuracy and generalization (lowest hamming loss across all models)

---

## 🏗️ System Architecture

```
Raw Comments (CSV)
        ↓
  Data Preprocessing
  (stopword removal, special character cleaning)
        ↓
  Count Vectorizer
  (word frequency vector)
        ↓
  ┌─────────────────────────────────────────┐
  │  SVM │ LR │ NB │ RF │ DT │ KNN         │
  └─────────────────────────────────────────┘
        ↓
  Accuracy / Loss Comparison
        ↓
  Predict on Test Comments
```

---

## 🧪 Classification Labels

Each comment can belong to **zero, one, or more** of the following categories (multi-label):

- `toxic`
- `severe_toxic`
- `obscene`
- `threat`
- `insult`
- `identity_hate`

---

## 🔧 Tech Stack

| Component        | Technology              |
|------------------|-------------------------|
| Language         | Python 3.7              |
| ML Library       | Scikit-learn            |
| Data Processing  | Pandas, NumPy           |
| Vectorization    | CountVectorizer         |
| Visualization    | Matplotlib              |
| Deep Learning    | TensorFlow              |
| UI               | Tkinter (Desktop GUI)   |

---

## 📁 Project Structure

```
major-project/
├── Dataset/
│   ├── train.csv          # Training dataset (custom, 65MB)
│   └── testComment.csv    # Test comments for prediction
├── Main.py                # Core ML pipeline and GUI
├── req.txt                # Python dependencies
└── run.bat                # Launch script (Windows)
```

---

## 🚀 How to Run

### Prerequisites
```bash
pip install -r req.txt
```

### Launch
```bash
# Windows
run.bat

# Or directly
python Main.py
```

### Steps in the Application
1. **Upload Toxic Comments Dataset** → loads `train.csv`
2. **Preprocess Dataset** → cleans comments (stopwords, symbols)
3. **Apply Count Vectorizer** → builds word frequency vectors
4. **Run Algorithms** → train SVM, LR, NB, RF, DT, KNN (80/20 split)
5. **Accuracy Comparison Graph** → visual comparison of all models
6. **Predict Toxic Comments** → upload `testComment.csv` for predictions

---

## 📈 Results

- Training/Testing split: **80% train / 20% test** (240 train, 60 test records)
- All 6 algorithms achieved accuracy **close to 95%+**
- Output labels: `[Contains TOXIC Comments]` or `[NOT CONTAINS TOXIC Comments]`

---

## 🔬 Methodology

1. **Data Cleaning** — Remove stopwords, special characters, normalize text
2. **Feature Extraction** — CountVectorizer to build word frequency matrix
3. **Multi-Label Classification** — Each comment can belong to multiple toxic categories
4. **Model Evaluation** — Accuracy, Log Loss, and Hamming Loss metrics
5. **Comparative Analysis** — All 6 algorithms evaluated on identical data splits

---

## 📚 Dataset

Custom preprocessed dataset stored in `Dataset/train.csv` (65MB).  
Based on the Jigsaw Toxic Comment Classification task with additional preprocessing applied.

> To use this project, clone the repo — the dataset is included in the repository.

---

## 🎓 Academic Context

**Project Type:** B.Tech Final Year Major Project  
**Domain:** Natural Language Processing / Machine Learning  
**Institution:** Malla Reddy Institute of Technology & Science, Hyderabad  
**Year:** 2023–2024

---

## 👤 Author

**Akshay Etukuri**  
B.Tech CSE (Networks) | MRITS Hyderabad  
[GitHub](https://github.com/AkshayEtukuri) | [LinkedIn](#)
