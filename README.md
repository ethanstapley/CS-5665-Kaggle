# Jigsaw Toxic Comment Severity Ranking – CS-5665 Final Project

This repository contains the final submission for the CS-5665 class project, built for the [Jigsaw Toxic Comment Severity Rating](https://www.kaggle.com/competitions/jigsaw-toxic-severity-rating) competition on Kaggle.

The goal is to assign a **relative toxicity score** to each online comment, such that the model agrees with expert annotators in ranking comments from least to most toxic.

---

## Repository Contents

| File | Description |
|------|-------------|
| `tf-idf-linear-regression.ipynb` | TF-IDF features with Linear Regression |
| `tf-idf-ridge-regression.ipynb`  | TF-IDF features with Ridge Regression |
| `tf-idf-lightgbm.ipynb`          | TF-IDF features with LightGBM |
| `tf-idf-random-forest-regressor.ipynb` | TF-IDF + Random Forest |
| `bert-score-sum.ipynb`           | Pretrained BERT model with weighted label summation |
| `ensemble.ipynb`                 | Ensemble of Ridge + BERT Score Sum |
| `train.csv`                      | Jigsaw training data (from previous competitions) |
| `validation_data.csv`           | Official validation pairs for scoring agreement |
| `comments_to_score.csv`         | Official test data (to be ranked) |
| `requirements.txt`              | Python packages for reproducibility |
| `Checkpoint 1.ipynb`                   | Checkpoint 1 |
| `Checkpoint 2.ipynb`                   | Checkpoint 2 |

---

## Environment Setup

Use Python 3.10+. To install required packages:

```bash
pip install -r requirements.txt
```

Pretrained Model:
This repository uses a personal pre-trained BERT model for toxicity scoring.

Download or use it directly from Kaggle:  
https://www.kaggle.com/models/ethanstapley/bert-toxic-epoch1/

Acknowledgement:
Some portions of the code in this project were generated or assisted by ChatGPT. This was used to accelerate development and ensure correctness. All generated code was reviewed, tested, and had human oversight.
