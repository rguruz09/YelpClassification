# YelpClassification

Motivation 

Review Services like Yelp, Google Reviews etc. provide customers and businesses a way to interact with one another. Reviews and Ratings are useful source of information but significant problem exists in extracting relevant information and predicting the future through analysis and correlation of the existing data. Yelp is currently the leading review service provider in the market. Each day thousands of restaurants and businesses are reviewed by the customers. Currently there is no efficient way to categorize the restaurants based on customer reviews. 

Objective 

In our project we try to predict category of the restaurant based on customer reviews. Our system will help other customers make decision on the restaurant to select based on the type of food they are interested in. The best way to categorise a restaurant is using customer reviews. The suggestions based on this approach are closer to the likings of the users. Our intention is to explore this approach and predict food category based on reviews that matches the actual food category. 


                                 System Design & Implementation details 
                                 
                                 
1. Algorithms considered/selected:

We have used KNN based approach for our classification model. We have also used K- fold cross validation (K=10) to validate our results. This algorithm helped us eliminate overfitting from our project. We have used PCA for dimensionality reduction. It is a simple, fast and efficient algorithm to reduce the size of our data set. 

2. Technologies & Tools used: 

We used Python as our programming language since it has many pre written libraries which can be used to perform KNN classification as well as 10 fold cross validation. To run our scripts we used jupyter notebook and also the command line occasionally. We have also used PyCharm IDE to develop the scripts. We have also used python libraries like Numpy, Scipy, NLTK, Pandas, Scikit-learn, Subprocess, Json etc. 

3. System design: 

Our system consists of multiple approach. Our initial Dataset is the raw data downloaded from Yelp. Then we filter out the data according to our requirements and store just the necessary dataset. Then we create a term frequency vector for our data and process the vector on our developed classification model. To further reduce the size of the data we perform dimensionality reduction on the vector. Then again we use the same model for classification. At the end we perform 10 fold cross validation on various dataset we had. The performance of all the approach was compared. 

Our System has following components: 

1. Data: Our data comes from Yelp. It contains 2.7M reviews and about 86K businesses. We then pre process the data. The result is two different datasets. One of them contains all the review text without common english words, stop words, punctuations etc. The second dataset contains all the review texts related to food words. 
Then we generate term frequency vector for both the approach. Dimensionality reduction is performed on both the vectors to generate two more vectors of reduced size. 

2. Classification Model: We then perform classification for the four datasets generated. Our classification model uses KNN based approach. We classify terms nearest to each other into a single label. 

3. 10 fold cross validation: To validate our results we perform 10 fold cross validation. Validation is necessary since we need to verify if our model generates the desired results or not. 

4. Performance Analysis: We compare the results and accuracy of all the four approach. We assess the performance and accuracy for our vectors 
