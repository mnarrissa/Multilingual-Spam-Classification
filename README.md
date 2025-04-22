1. About:
- This project enhances multilingual spam detection using DistilBERT embeddings and classical ML models (XGBoost, SVM, etc.). It supports 5 languages (English, Spanish, Arabic, Russian, Portuguese) and outperforms traditional single-language approaches. The stopwords for each language are located in the arabic.txt, spanish.txt, russian.txt, and portuguese.txt files.

2. Key Features:

- Multilingual Support: Preprocessing and classification for diverse languages.
- State-of-the-Art Models: XGBoost, SVM, Logistic Regression, and more.
- Explainability: SHAP analysis for model transparency.
- High Accuracy: Achieves 96.07% accuracy on combined multilingual data.

3. How to Run
- Data Preparation
  - Place your dataset in data/ (CSV format with text and labels columns).
  - Ensure stopword files (e.g., arabic.txt) are in data/.

2. Execute the Main Script
- Run python main.py
- This will:
  - Preprocess text (language-specific cleaning, tokenization).
  - Extract embeddings using DistilBERT.
  - Train & evaluate 7 ML models (XGBoost, SVM, etc.).
  - Generate ROC curves and SHAP analysis.

3. Results & Performance
- Best Model (XGBoost on Combined Data)
- Best model for English, Spanish, Arabic is SVM and for Russian and Portuguese is XGBoost

4. Key Improvements Over Baseline
- Multilingual Support (vs. English-only in prior work)
- Higher Robustness (XGBoost + DistilBERT vs. Logistic Regression)
- Explainable AI (SHAP analysis for model transparency)

5. Future Work
- Fine-tune DistilBERT for low-resource languages (Arabic/Russian).
- Deploy as an API for real-time spam filtering.
- Expand to more languages (e.g., Chinese, Hindi).
