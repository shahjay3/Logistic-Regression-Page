## Twitter Sentiment Analysis using Naive Bayes and K-Nearest Neighbors

### MOTIVATION FOR THE PROJECT
Companies all over are looking for better ways to connect with their customers. A common way to do this is to use social media to extract information about how customers view a new product. To quantify this, using sentiment analysis could yield valuable information. This project will use text mining techniques to classify tweets as a positive sentiment or negative sentiment tweet to gain information on how users view a particular product. 

We thought that it would be fun to use two classificaiton algorithms applied ot twitter sentiment.

### ALGORITHMS FOR THE PROJECT

We use two algorithms to classify tweets into one of two sentiment classes: postive sentiment, which is characterized by a lexicon that consists of only positve words, and negative sentiment, which consists of commonly used negative words.

The classification algorithms that we decided to use are Naive Bayes and K-Nearest Neighbor Algorithm.
Naieve Bayes is a classification algorithm that uses prior probabilites in order to classify new doucments into a particular class. We use this technique with smooth, with the alpha paramter of 1. The alpha parameter is there to account for those words that are non-existant in each class, thus giving it a preliminary weight of one. This prevents any calculated probability to be 0 when there is at least one word in the twitter document that doesn't belong to a sentiment class. 

For K-NN, in order to find the nearest neighbor, we use cosine similarity. When strive to develop a numerical vector repreentaiton of each tweet. We do this by 

### DATA SET FOR THE PROJECT

The data set will be obtained by using the Twitter API streaming functionality in Python. The training set will consist of over 600,000 positive tweets as well as 600,000 negative tweets obtained by tracking common positive and negative words as well as emoticons. All testing tweets will be obtained the using the Twitter real time Streaming API.

### WHAT WE PLAN TO ACCOMPLISH

What are we going to accomplish? We will accomplish implementing both Naive Bayes and K-NN classification to classify tweets relating to President Trump and United Airlines Scandal. : This was completed. Naive Bayes classification yeilded an 80% accuracy when comparing pre-labeled tweets relating to trump. 

What are we likely to accomplish? Extend our binary Naïve Bayes classifier to a Multinomial Naive Bayes classifier that considers more than two emotion classes to classify tweets. 

What will we ideally like to accomplish? 
We would like to make this into a real time system that automatically classifies tweets as positive/negative sentiments as they are grabbed from twitter, as well show sentiments as a function of geographic location (preferably on a map). 

### RESULTS 

For the Naive Bayes Classifier, we achieved an 80% accuracy when comparing pre-labeled 1000 tweets relating to trump vs the classified tweets relating to trump. Majority of the trump tweets, when pre-labeling, were of negative sentiment. When we ran our Naive Bayes Classifier, we also found that majority of sentiments belong to the negative sentiment class. 

For the KNN classifier, we achieved

### Division of Responsibilities 
a.	***Jay Shah***: Training/Testing the Naïve Bayes Classifier, Grabbing Tweets for negative sentiments, cleaning the tweets : Achieved

b.	***Nanda Kishore Kolluru***: Training/ Testing the K-NN Classifier, Grabbing Tweets for positive sentiments, cleaning and processing the tweets for analysis. : Achieved

c.	***Both***: Work on Logistic Regression and Work on real time system that classifies tweets as they come in: Logistic Regression was carried out however, we encontered many problems with. 

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for 

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/shahjay3/Logistic-Regression-Page/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
