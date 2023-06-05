To perform exploratory data analysis (EDA) on the given dataset, the code provided can be used. Here's an explanation of the code and its outputs:

```python
# Checking for missing values in the dataset
df.isnull().sum()
```
This code checks for missing values in the DataFrame `df` and returns the count of missing values for each column.

```python
# Counting the occurrences of each sentiment
sentiment_count = Counter(df['Sentiment'])
print(sentiment_count)
```
This code uses the `Counter` class from the `collections` module to count the occurrences of each sentiment in the 'Sentiment' column of the DataFrame `df`. The output is a dictionary with sentiment labels as keys and their corresponding counts as values. It is then printed to the console.

```python
# Plotting the distribution of sentiments
sns.countplot(x='Sentiment', data=df)
plt.title('Distribution of Sentiments')
plt.show()
```
This code uses the `countplot` function from the `seaborn` library to create a bar plot of the distribution of sentiments in the DataFrame `df`. The x-axis represents the sentiment labels, and the height of each bar represents the count of occurrences for each sentiment. The plot is then displayed with a title.

```python
# Calculating the length of each text in the data
df['text_length'] = df['Text'].apply(len)
```
This code calculates the length of each text in the 'Text' column of the DataFrame `df` using the `apply` function with the `len` function as the argument. The resulting lengths are stored in a new column called 'text_length'.

```python
# Plotting the distribution of text lengths
sns.histplot(x='text_length', data=df)
plt.title('Distribution of Text Lengths')
plt.show()
```
This code uses the `histplot` function from the `seaborn` library to create a histogram of the distribution of text lengths in the DataFrame `df`. The x-axis represents the text lengths, and the height of each bar represents the count of texts with a particular length. The plot is then displayed with a title.

```python
# Plotting the relationship between text length and sentiments
sns.histplot(x='text_length', data=df, hue='Sentiment', multiple='stack')
plt.title('Distribution of Text Lengths by Sentiment')
plt.show()
```
This code creates a histogram similar to the previous one, but this time it distinguishes the sentiment labels by different colors using the `hue` parameter. The `multiple='stack'` parameter stacks the bars for different sentiments on top of each other. The plot is then displayed with a title.

