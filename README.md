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


