# Text Classification and Topic Modeling

## Overview
This project focuses on two primary tasks using the **economic_news.xlsx** dataset:

1. **Text Classification:** Determining whether a news article is relevant to business ("Yes") or not ("No").
2. **Topic Modeling:** Identifying key topics present within the news articles.

## Dataset
- **File:** `economic_news.xlsx`
- **Description:** Contains news articles with corresponding labels indicating their relevance to business.
- **Columns:**
  - `Headline`: Title of the news article
  - `Text`: Full content of the article
  - `Relevant`: Target variable ("Yes" or "No")

## Task 1: Text Classification

### Algorithms Used
- **Logistic Regression**
- **Random Forest Classifier**
- **Naive Bayes Classifier**

### Evaluation Metrics
- **Confusion Matrix**
- **Classification Report** (Precision, Recall, F1-score)

### Model Interpretation
- **LIME (Local Interpretable Model-agnostic Explanations):**
  - Highlights words that are strong predictors of relevance/irrelevance.

## Task 2: Topic Modeling

### Techniques Used
- **Non-Negative Matrix Factorization (NMF)**
- **Latent Semantic Analysis (LSA) using TruncatedSVD**
- **Latent Dirichlet Allocation (LDA)**

### Output
- **10 Topics** identified from the combined `Headline` and `Text` columns.
- **Top 20 Words** displayed for each topic to understand thematic structures.

## Project Structure
```
├── data
│   └── economic_news.xlsx
├── notebooks
│   ├── text_classification.ipynb
│   └── topic_modeling.ipynb
├── models
│   └── saved_models.pkl
├── visualizations
│   └── lime_explanations.png
├── requirements.txt
└── README.md
```

## Requirements
Install the dependencies using:
```bash
pip install -r requirements.txt
```

### Key Libraries
- `pandas`, `numpy`
- `scikit-learn`
- `matplotlib`, `seaborn`
- `lime`
- `nltk` or `spaCy` (for text preprocessing)

## Running the Project
1. **Text Classification:** Open and run `text_classification.ipynb` to train models and visualize results.
2. **Topic Modeling:** Execute `topic_modeling.ipynb` to extract topics and analyze key words.

## Results
- **Classification Models:** Comparative performance analysis.
- **LIME Interpretations:** Insights into influential words.
- **Topic Modeling:** Clear representation of prevalent topics in economic news.

## Acknowledgments
Thanks to all contributors and open-source libraries that supported this project.

---
Feel free to fork, contribute, or raise issues!

