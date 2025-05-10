# Click-Through Rate (CTR) Prediction using Deep Learning

This project focuses on predicting the Click-Through Rate (CTR) for online advertisements using advanced deep learning models. The dataset is provided by **Avazu**, an advertising company, as part of a Kaggle competition.

## 📊 Project Overview

The objective is to build models that accurately predict whether a user will click on a given advertisement, using anonymized user and ad features.

## 🗂 Dataset

- **Source**: [Avazu CTR Prediction - Kaggle](https://www.kaggle.com/c/avazu-ctr-prediction)
- **Description**: Contains click logs including various categorical and timestamped features.
- **Size**: ~24 GB uncompressed

## 🔍 Exploratory Data Analysis (EDA)

Performed EDA to:
- Understand feature distribution
- Analyze click-through behavior over time
- Encode categorical features
- Detect data imbalance

## 🧠 Models Used

Four deep learning models were implemented and compared:

1. **DeepFM (Deep Factorization Machine)**
   - Combines FM and DNN to model both low- and high-order feature interactions.

2. **xDeepFM (eXtreme DeepFM)**
   - Enhances DeepFM using a Compressed Interaction Network (CIN) to model explicit feature interactions.

3. **WDL (Wide & Deep Learning)**
   - A hybrid model that leverages linear (wide) and deep neural network (deep) components.

4. **DCN (Deep & Cross Network)**
   - Captures cross-feature interactions via Cross Network layers, improving generalization.

## 🛠️ Tools & Libraries

- Python
- TensorFlow / PyTorch
- Pandas, NumPy
- Matplotlib, Seaborn (for visualization)
- Scikit-learn (for preprocessing and metrics)

## ✅ Test Accuracy Scores

| Model     | Test Accuracy |
|-----------|----------------|
| DeepFM    | 0.8308         |
| XDeepFM   | 0.8306         |
| WDL       | 0.8120         |
| DCN       | 0.8161         |

## ⚙️ Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/amirtha-lab-27/click-through-rate
   cd ctr-prediction-avazu
