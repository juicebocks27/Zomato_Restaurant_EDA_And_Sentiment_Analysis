One of the most used learning algorithms in ML is Unsupervised Learning. Unsupervised learning models are utilised for three main tasks—clustering, association, and dimensionality reduction. In this project, we perform a clustering exercise and then do the sentimental analysis to extract customer reviews.

This problem contains two data frames -
* Zomato restaurant data contains all information about the available restaurants on Zomato, the cuisines they serve, the per-person cost of dining, etc.
* User review collection contains users' ratings and reviews of different restaurants.

Food apps like Zomato are widely used because they not only serve food to the door but also provide a platform for people to share their opinion about the restaurants and cafes they have visited. 

The project focuses on analysing the Zomato restaurant data for each city in India and grouping them into clusters. Also, explore the reviews given for the particular restaurant by the reviewers to determine if they have positive or negative sentiments towards the dish/restaurant.

Started with text data Preprocessing ( Using NLP)

Firstly I performed the clustering on the hotel dataset but before clustering, I did dimensionality reduction using Principal Component Analysis and applied three algorithms. The models implemented are :

* K Means clustering
* Agglomerative Hierarchical clustering
* DBSCAN

Found that data can be divided into 6 clusters. Using the Silhouette score, I checked the score of KMeans and Hierarchical clustering.

Next is Sentiment Analysis for the review dataset. For sentiment analysis, first, I performed Textual data preprocessing. This involves Punctuation Mark Removal, Stop Word Removal, Lemmatization, handling emojis, converting to lowercase, and tokenisation. For tokenisation, I used tf-idf vectoriser.

Models performed for sentiment analysis are

* Logistic Regression
* DecisionTree
* Random Forest
* XGBoost Classifier
* K Nearest Neighbour

And I inferred that logistic regression performs best among all other models considering the AUC_ROC score. I also did hyperparameter tuning and concluded that Logistic regression could be deployed for the final prediction of Sentiment Analysis.
