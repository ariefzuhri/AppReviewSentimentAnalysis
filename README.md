# 💬 NLP Sentiment Analysis of Mobile App Reviews

A deep-learning NLP pipeline that turns multilingual ELSA Speak app reviews into balanced sentiment data and predicts positive/negative user sentiment.

## ⚙️ What I Built

- Collected **91K+ Google Play reviews** across English, Vietnamese, Indonesian, and Arabic.
- Translated non-English reviews to English and built a reusable text-cleaning pipeline.
- Normalized contractions, punctuation, emojis, whitespace, and lemmatization; removed blank and cross-language duplicates.
- Used **fastText** for language validation and **RoBERTa** for confidence-based sentiment labeling.
- Compared star ratings, VADER, and RoBERTa to improve label quality.
- Built balanced 3-class and binary datasets with stratified train/validation/test splits.
- Trained and compared **TF-IDF + Dense NN** and **TF-IDF + class-weighted Dense NN** approaches, with checkpointing and early stopping.
- Added a lightweight inference workflow for new reviews with confidence scores.

## 🛠️ Tech Stack

**Python · Pandas · NumPy · scikit-learn · TensorFlow/Keras · Transformers · RoBERTa · TF-IDF · fastText · NLTK · VADER · Matplotlib · Jupyter Notebook**

## 🤖 Result

- **Best model:** Binary TF-IDF + Dense Neural Network.
- **Test Accuracy:** **87.14%**.
- **Macro F1:** **85.99%**.
- **Negative F1:** 81.97% - **Positive F1:** 90.01%.
- Demonstrated reliable separation of clear positive/negative reviews while exposing ambiguity through prediction confidence.

## ✨ Key Takeaway

Built an end-to-end NLP workflow that combines **data engineering, weak labeling, dataset balancing, model experimentation, evaluation, and practical inference** into one reproducible sentiment-analysis pipeline.
