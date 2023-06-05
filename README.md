# Title: Stock Market Sentiment Analysis Using Machine Learning and BERT Transformer Model

## Abstract:

Accurate prediction of stock market sentiment is crucial for informed decision-making by investors and financial analysts. In this research study, we explore the application of various machine learning (ML) models to analyze sentiment in stock market data. We employ five traditional ML models and leverage advanced deep learning techniques, including the powerful Transformer model, BERT.

Our research aims to compare the performance of these models in accurately predicting stock market sentiment. We evaluate their performance using commonly used evaluation metrics and analyze their strengths and weaknesses based on interpretability, robustness to noise, and ability to capture complex patterns in the text data.

Among the models tested, BERT using TF-IDF achieved the highest accuracy of approximately 83%. This result demonstrates the effectiveness of BERT in capturing nuanced sentiment in stock market data. Additionally, we provide insights into the interpretability of the models, their resilience to noisy data, and their capacity to detect complex patterns.

The findings of this research contribute to the field of stock market sentiment analysis by highlighting the potential of both traditional ML models and advanced deep learning techniques. The comparison and evaluation of these models provide valuable guidance to investors and financial analysts in making informed decisions based on sentiment analysis of stock market data.

# Stock Market Sentiment Analysis using Machine Learning Models and BERT Transformer

This research study focuses on the accurate prediction of stock market sentiment using various machine learning (ML) models and the powerful BERT Transformer model. We evaluate the performance of these models, both with and without hyperparameter tuning, and compare their effectiveness in capturing sentiment in stock market data. Additionally, we provide insights into the interpretability, robustness to noise, and ability to capture complex patterns of these models.

## Model Performance

### Vectorization

| Model               | Without Hyperparameter Tuning | With Hyperparameter Tuning |
|---------------------|-------------------------------|----------------------------|
| Linear Regression   | 0.22                          | NAN                        |
| Logistic Regression | 0.78                          | 0.8                        |
| TF-IDF + KNN         | 0.76                          | 0.75                       |
| TF-IDF + Decision Tree | 0.73                        | 0.73                       |
| TF-IDF + Random Forest | 0.79                        | 0.65                       |
| Neural Network      | 0.7972                        |                            |
| BERT                | ~83 (best)                    |                            |

### Bag-of-Words (BOW)

| Model               | Without Hyperparameter Tuning | With Hyperparameter Tuning |
|---------------------|-------------------------------|----------------------------|
| Linear Regression   | 0.18                          | NAN                        |
| Logistic Regression | 0.79                          | 0.79                       |
| BOW + KNN           | 0.68                          | 0.68                       |
| BOW + Decision Tree | 0.73                          | 0.74                       |
| BOW + Random Forest | 0.79                          | 0.65                       |

Please refer to the [Kaggle notebook](https://www.kaggle.com/code/pratyushpankaj/stock-market-sentiment-analysis#PLOT-OF-ALL-MODELS) for a detailed visualization of all the models.

## Model Information

### Linear Regression

- Accuracy without hyperparameter tuning: 0.22 (Vectorization) / 0.18 (BOW)
- Accuracy with hyperparameter tuning: NAN (Vectorization) / NAN (BOW)

### Logistic Regression

- Accuracy without hyperparameter tuning: 0.78 (Vectorization) / 0.79 (BOW)
- Accuracy with hyperparameter tuning: 0.8 (Vectorization) / 0.79 (BOW)

### TF-IDF + KNN

- Accuracy without hyperparameter tuning: 0.76 (Vectorization) / 0.68 (BOW)
- Accuracy with hyperparameter tuning: 0.75 (Vectorization) / 0.68 (BOW)

### TF-IDF + Decision Tree

- Accuracy without hyperparameter tuning: 0.73 (Vectorization) / 0.73 (BOW)
- Accuracy with hyperparameter tuning: 0.73 (Vectorization) / 0.74 (BOW)

### TF-IDF + Random Forest

- Accuracy without hyperparameter tuning: 0.79 (Vectorization) / 0.79 (BOW)
- Accuracy with hyperparameter tuning: 0.65 (Vectorization) / 0.65 (BOW)

### Neural Network

- Accuracy: 0.7972 (Vectorization)

### BERT Transformer

- Best Accuracy: ~83% (Vectorization)

## Conclusion

In this study, we explored various machine learning models and the BERT Transformer model for stock market sentiment analysis. The results demonstrate that BERT, when using TF-IDF vectorization, achieved the highest accuracy of approximately 83%. Logistic regression and random forest models also exhibited competitive performance. The models' interpretability, robustness to noise, and ability to capture complex patterns varied across the different approaches.
