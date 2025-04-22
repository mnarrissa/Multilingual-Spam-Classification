This project enhances multilingual spam detection using DistilBERT embeddings and classical ML models (XGBoost, SVM, etc.). It supports 5 languages (English, Spanish, Arabic, Russian, Portuguese) and outperforms traditional single-language approaches. The stopwords for each language are located in the arabic.txt, spanish.txt, russian.txt, and portuguese.txt files.

- Key Features:

1. Multilingual Support: Preprocessing and classification for diverse languages.

2. State-of-the-Art Models: XGBoost, SVM, Logistic Regression, and more.

3. Explainability: SHAP analysis for model transparency.

4. High Accuracy: Achieves 96.07% accuracy on combined multilingual data.

- How to Run
1. Data Preparation
a. Place your dataset in data/ (CSV format with text and labels columns).

b. Ensure stopword files (e.g., arabic.txt) are in data/.

2. Execute the Main Script
a. run python main.py

b. This will:

  - Preprocess text (language-specific cleaning, tokenization).

  - Extract embeddings using DistilBERT.

  - Train & evaluate 7 ML models (XGBoost, SVM, etc.).

  - Generate ROC curves and SHAP analysis.

- Results & Performance
1. Best Model (XGBoost on Combined Data)
2. Best model for English, Spanish, Arabic is SVM and for Russian and Portuguese is XGBoost

- Key Improvements Over Baseline
1. Multilingual Support (vs. English-only in prior work)
2. Higher Robustness (XGBoost + DistilBERT vs. Logistic Regression)
3. Explainable AI (SHAP analysis for model transparency)

- Future Work
1. Fine-tune DistilBERT for low-resource languages (Arabic/Russian).
2. Deploy as an API for real-time spam filtering.
3. Expand to more languages (e.g., Chinese, Hindi).
