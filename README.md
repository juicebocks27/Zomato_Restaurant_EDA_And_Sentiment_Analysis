One of the mostly used learning in ML is Unsupervised Learning. Unsupervised learning models are utilized for three main tasks—clustering, association, and dimensionality reduction. In this project we perform clustering exercise and then do the sentimental analysis to extract reviews from customers.

This problem contain two dataframes -
* Zomato restaurant data which contains all information about the restaurants that are available on Zomato, cuisines they serve, per person cost of dining, etc.
* User review collection which contains the ratings and reviews given by users to different restaurants.

Food apps like Zomato are widely used because it not only serves food to the door but also provides a platform for people to share their opinion about the restaurants and cafes they have visited. 

The project focuses on analysing the Zomato restaurant data for each city in India and grouping them into clusters. Also analyze the reviews given for the particular restaurant by the reviewers to find out if they have positive sentiment or negative sentiment towards the dish/restaurant.

Firstly I performed the clustering on hotel dataset but before clustering I did dimensionality reduction using Principal Component Analysis and applied 3 algorithms. The models implemented are :

* K Means clustering
* Agglomerative Hierarchical clustering
* DBSCAN

And found that data can be divided into 6 clusters. Using Sillhoutte score, checked the score of KMeans and Hierarchichal clustering.

Next is Sentiment Analysis for review dataset. For sentiment analysis, first I performed Textual data preprocessing. This involves steps like Punctuation Mark Removal, Stop Word Removal, Lemmatization, handling emojis, converting to lower case, tokenization. For tokenization, I used tf-idf vectorizer.

Models performed for sentiment analysis are

* Logistic Regression
* DecisionTree
* Random Forest
* XGBoost Classifier
* K Nearest Neighbour

And inferred that logistic regression is performing best among all other models considering AUC_ROC score. Also did hyperparameter tuning and concluded that Logistic regression can be deployed for final prediction of Sentiment Analysis.
