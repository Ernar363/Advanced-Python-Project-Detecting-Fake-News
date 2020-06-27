# Advanced-Python-Project-Detecting-Fake-News
This advanced python project of detecting fake news deals with fake and real news. Using sklearn, we build a TfidfVectorizer on our dataset. Then, we initialize a PassiveAggressive Classifier and fit the model. In the end, the accuracy score and the confusion matrix tell us how well our model fares.

# The Dataset
The dataset we’ll use for this python project- we’ll call it news.csv. This dataset has a shape of 7796×4. The first column identifies the news, the second and third are the title and text, and the fourth column has labels denoting whether the news is REAL or FAKE.

# Prerequisites
I’ll need to install the following libraries with pip:
[Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/1.png)

I’ll need to install Jupyter Lab to run your code. Get to your command prompt and run the following command:
[Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/2.png)

1. Made the import of the necessary libraries for the project:
[Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/3.png)

2. Now, let’s read the data into a DataFrame, and get the shape of the data and the first 5 records:
[Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/4.png)
Output Screenshot: [Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/5.png)

3. Then get the tags from the DataFrame:
[Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/6.png)
Output Screenshot: [Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/7.png)

4. I divide the data set into training and test sets.
[Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/8.png)
Output Screenshot: [Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/9.png)

5. Now initialize TfidfVectorizer using stop words from the English language and a maximum frequency of documents of 0.7 (terms with a higher frequency of documents will be discarded). Stop words are the most common words in a language that need to be filtered out before processing data in a natural language. And TfidfVectorizer turns a collection of raw documents into a matrix of TF-IDF functions.

Now install and convert the vectorizer into a set of trains and convert the vectorizer into a test set.
Output Screenshot: [Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/10.png)

6. Next, we’ll initialize a PassiveAggressiveClassifier.
Then, I’ll predict on the test set from the TfidfVectorizer and calculate the accuracy with accuracy_score() from sklearn.metrics.
[Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/11.png)
Output Screenshot: 
[Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/12.png)

7. I got an accuracy of 92.74% with this model. Finally, let’s print out a confusion matrix to gain insight into the number of false and true negatives and positives:
[Image](https://github.com/Ernar363/Advanced-Python-Project-Detecting-Fake-News/raw/master/images/13.png)

So with this model, we have 590 true positives, 585 true negatives, 44 false positives, and 48 false negatives.

# Summary
Today, I learned to detect fake news with Python. I took a political dataset, implemented a TfidfVectorizer, initialized a PassiveAggressiveClassifier, and fit our model. We ended up obtaining an accuracy of 92.74% in magnitude.
