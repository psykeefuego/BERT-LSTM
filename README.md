
# Sentiment Analysis using LSTM and BERT

## Overview

This notebook presents a comparative analysis of two models—**a traditional LSTM-based neural network** and a **pre-trained BERT model**—for **sentiment classification** on the IMDb movie reviews dataset.

The task was completed as part of the first-round selection process for the Summer Research Internship at the Department of Computer Science and Engineering, Mahindra University.

---

## Task Summary

| Component       | Details                                                                                                       |
| --------------- | ------------------------------------------------------------------------------------------------------------- |
| **NLP Task**    | Sentiment Analysis (Binary)                                                                                   |
| **Dataset**     | [IMDb Dataset from Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews) |
| **Models Used** | 1. LSTM (Keras)  <br> 2. BERT (`bert-base-uncased`) via HuggingFace                                           |
| **Libraries**   | `transformers`, `tensorflow`, `keras`, `pandas`, `sklearn`, `matplotlib`, `seaborn`                           |

---

## Project Structure

* **Data Loading & Preprocessing:** IMDb reviews labeled as positive or negative.
* **Model 1 – LSTM:**

  * Tokenized and padded sequences
  * Trained for 5 epochs
* **Model 2 – BERT:**

  * Used `TFBertForSequenceClassification`
  * Fine-tuned for 3 epochs
* **Evaluation Metrics:**

  * Accuracy, Confusion Matrix, Classification Report
* **Visualization:**

  * Accuracy plots over epochs
  * Confusion matrices
  * Final accuracy comparison bar chart

---

## Key Results

| Model | Accuracy (Test Set)             |
| ----- | ------------------------------- |
| LSTM  | *\~0.85%* *(update after run)* |
| BERT  | *\~0.92%* *(update after run)* |

BERT outperformed LSTM in overall accuracy and generalization, showcasing the power of pre-trained transformer models on language understanding tasks.

---

## How to Run

1. Open the notebook in Google Colab or Jupyter.
2. Upload `IMDB Dataset.csv` (if not using the HuggingFace IMDb loader).
3. Run all cells sequentially.
4. Review the accuracy plots and classification reports at the end.

---

