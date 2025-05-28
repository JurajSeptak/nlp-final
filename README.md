# 🎵 Do Words Make Hits? An Application of NLP in Song Popularity Prediction

This project explores whether song lyrics and audio features can predict the chart success of songs on U.S. Billboard rankings using Natural Language Processing (NLP) and machine learning techniques.

## 📂 Project Structure

- `1. Data cleaning & Feature engineering.ipynb`  
  Scripts for loading, merging, and preprocessing Spotify and Billboard datasets. Includes filtering English lyrics and generating audio and lexical features.

- `2.EDA.ipynb`  
  Exploratory data analysis of audio and text features. Includes distribution visualizations, clustering attempts, and linguistic insights.

- `3. Model Training.ipynb`  
  Training scripts for various classifiers (LogReg, RF, NB, MLP) across multiple feature sets (audio, lexical, lyrics). Includes embeddings with TF-IDF, Bag-of-Words, and SBERT.

- `training_sets/`  
  Contains all pre-split datasets (train/val/test) for each feature configuration (A, L, T, L_T, L_A, T_A, A_L_T).

## 🧪 Models & Techniques

- **Feature Types:**  
  - Audio attributes (e.g., danceability, energy, valence)  
  - Lexical features (e.g., vocab size, repetition ratio)  
  - Raw and embedded lyrics (BoW, TF-IDF, SBERT)

- **Classification Models:**  
  Logistic Regression, Naive Bayes, Random Forest, Multilayer Perceptron

- **NLP Tools:**  
  `spacy`, `nltk`, `sentence-transformers`, `scikit-learn`, `gensim`

- **Imbalance Handling:**  
  SMOTE and ADASYN oversampling techniques applied to address class imbalance in hit vs. non-hit labels.

## 📈 Reproducibility

- Python 3.10 environment with exact versions listed in notebooks  
- Random seed fixed at `42` for all train/val/test splits and models  
- All intermediate datasets and embeddings are saved to avoid recomputation  
- Consistent preprocessing across all splits (lyrics checked for consistency)

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/spotify-hit-prediction-nlp.git
   cd spotify-hit-prediction-nlp
   ```

2. Set up the environment:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebooks in order:
   - `1. Data cleaning & Feature engineering.ipynb`
   - `2. EDA.ipynb`
   - `3. Model Training.ipynb`

## 🧑‍💻 Authors

- Beatriz Alessandra Tomasoni Jorquera  
- Sara Recio Cristobal  
- Juraj Septak

MSc Business Administration and Data Science, 2025  
Copenhagen Business School
