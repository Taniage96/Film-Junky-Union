# Film Junky Union - Automated Movie Review Classification

## Project Overview

Film Junky Union, a new and innovative community for classic film enthusiasts, aims to develop a system for filtering and categorizing movie reviews. This project focuses on training a model to automatically detect negative reviews using an IMDB movie review dataset. The goal is to build a robust classifier that accurately distinguishes between positive and negative reviews, enhancing the user experience on the platform.

## Methodology

### Data Preprocessing

* **Data Loading:** IMDB movie reviews were loaded from a TSV file into a Pandas DataFrame.
* **Text Preprocessing:**
    * Lowercasing: Converted all text to lowercase.
    * Tokenization: Split text into individual words or tokens.
    * Lemmatization: Reduced words to their base or dictionary form.
    * Stop Words Removal: Eliminated common words that do not contribute significantly to the meaning.
* **Feature Engineering:**
    * TF-IDF Vectorization: Transformed textual data into numerical features using Term Frequency-Inverse Document Frequency.

### Model Selection

* **Baseline Models:**
    * Logistic Regression
    * LightGBM
    * Dummy Classifier (for baseline comparison)
* **Advanced Models:**
    * Neural Network (TensorFlow/Keras)
    * BERT (Bidirectional Encoder Representations from Transformers) using the `transformers` library.

### Training and Evaluation

* **Data Splitting:** The dataset was divided into training and testing subsets.
* **Cross-Validation:** Stratified KFold cross-validation was employed to ensure consistent model performance across different data segments.
* **Hyperparameter Tuning:** Grid search was used to optimize model hyperparameters.
* **Evaluation Metrics:**
    * Accuracy
    * Precision
    * Recall
    * F1 Score
    * AUC-ROC
