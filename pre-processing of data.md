## Dataset

The dataset used for sentiment analysis consists of two columns: 'Text' and 'Sentiment'. The 'Text' column contains the stock market-related text, while the 'Sentiment' column represents the sentiment of the text as either 1 (positive) or -1 (negative).

## Preprocessing

Before training the machine learning models, the dataset undergoes several preprocessing steps to clean and prepare the text data. The following preprocessing steps are applied to the 'Text' column:

- Removal of non-alphanumeric characters
- Removal of single character words
- Removal of single characters at the beginning of the text
- Replacement of multiple spaces with a single space
- Conversion to lowercase

Stop words and punctuation are also removed using the `en_core_web_sm` model from spaCy. The preprocessed text is stored in the 'text_processed' column.

## Stemming

Stemming is applied to further reduce the dimensionality of the text data. The Porter stemming algorithm is used to transform words to their base or root form. Stop words are also removed during stemming.

## Vectorization

Two different vectorization techniques are explored: Term Frequency-Inverse Document Frequency (TF-IDF) and Bag of Words (BoW). TF-IDF assigns weights to words based on their frequency and importance in the text corpus, while BoW represents text as a collection of word counts.

## Machine Learning Models

Five machine learning models are used for sentiment analysis:

1. Linear Regression
2. Logistic Regression
3. Decision Tree
4. Random Forest
5. K-Nearest Neighbors (KNN) Classification

Additionally, three deep learning models are utilized:

1. Basic Neural Network
2. Long Short-Term Memory (LSTM)
3. Transformers (BERT)

The models are trained and evaluated using the preprocessed and vectorized data.

## Evaluation Metrics

The accuracy score is used as the evaluation metric to measure the performance of the machine learning models. The accuracy is calculated by comparing the predicted sentiment labels with the true labels.

## Requirements

The following dependencies are required to run the code in this repository:

- pandas
- numpy
- matplotlib
- seaborn
- nltk
- spacy
- scikit-learn
- tensorflow
- transformers

## Usage

To run the code, follow these steps:

1. Install the required dependencies.
2. Clone the repository to your local machine.
3. Load the dataset and ensure it is in the correct format (with 'Text' and 'Sentiment' columns).
4. Run the preprocessing steps to clean and prepare the text data.
5. Perform exploratory data analysis to gain insights into the dataset.
6. Generate word clouds to visualize the most common words in positive and negative sentiment texts.
7.

 Apply stemming to further process the text data.
8. Balance the dataset to address class imbalance.
9. Vectorize the preprocessed text data using either TF-IDF or BoW.
10. Train the machine learning models and evaluate their performance.
11. Explore the deep learning models for sentiment analysis.

Please refer to the individual code files for more detailed instructions and explanations.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Feel free to use the code and data provided in this repository for your own analysis and research.
