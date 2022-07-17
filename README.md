Sentiment-Analysis

INTRODUCTION:

It is a project based on Natural Language Processing(NLP) that deals with devlopment of various applications that can be used by machine to decode the Human Language.

NLP can be defined as the process of translating Textual data into meaningful data.

NLP uses the Natural Language Tool Kit(NLTK) which is a very powerful NLP library that consists of packages that help machine understand the human language.

There are basic three processes involved in NLP.

⦁	The first process is related with Data Cleaning.
	Data cleaning consists of multiple steps such as Tokenization,Stop word removal,Stemming and Lemmatization.
  
⦁	The second process deals with Vectorization.

⦁	The third process is related with Data Classification.
  Data classification is known as text tagging or text categorization.


PROCESS:

1.Data Cleaning: Cleaning the raw data.

⦁	Tokenization is defined as the process of dividing the entire document or paragraph into smaller units of individual words or phrases. These smaller units are called Tokens.

⦁	Stop Word Removal is the process of removing those words or phrases whose presence has no effect on the overall analysis of the data.

⦁	Stemming is the process of converting the words to its roots.The project uses the Porter Stemming process for the purpose of stemming.


2. Vectorization: Mapping of words or phrases to a vector of real numbers.

3.Data Classification: Categorizing the data into individual groups.
  Data Classification is based on the Naive Bayes Algorithm.


NAIVE BAYES ALGORITHM:

Naive bayes algorithm is based on the Bayes theorom of mathematics that deals with the Conditional Probability of the data.
According to Naive Bayes algo, "Probability of event A to occur when B has already occured is equal to the product of Posterior probability and Prior Probability"


LIBRARIES USED:

⦁	Tokenization process uses the "RegexpTokenize" library of "nltk.tokenize" package.

⦁	Stop word removal technique uses the "StopWords" library of the "nltk.corpus" package.

⦁	For stemming the project uses the Porter Stemmer Method.
  
  It uses the "PorterStemmer" library of the "nltk.stem.porter" package.
  
![image](https://user-images.githubusercontent.com/70806075/177722870-9777e492-fa2f-43ad-aeee-669c9ce8e2de.png)


⦁	Vectorization uses the "CountVectorizer" library of the "sklearn.feature_extraction.text" package.
![image](https://user-images.githubusercontent.com/70806075/177723917-2d6335b8-5cc5-414f-94e6-74878db23109.png)

⦁	For Classification purpose the project uses the MULTINOMIAL NAIVE BAYES algorithm.
  
  It uses the "MultinomialNB" library of the "sklearn.naive_bayes" package.
![image](https://user-images.githubusercontent.com/70806075/177724147-9257ab15-c377-46a3-a2cf-eba4eea81b52.png)

TRAINING THE MODEL:

The project uses a train data so as to train the model.This model has been uploaded from Kaggle famed as 'Amazon headphones review'. This train data consists of several sentences correalted with customer's reviews on different headphones available in the market, feeded to the system so that they can be recognised as sentiments of positivity or negativity.

This data set is used to help machine understand the basic words which are used by each and every individual to share his experiences.
Following is the data set uploaded in the model by using pandas library of python.
![image](https://user-images.githubusercontent.com/70806075/179391367-4881e293-0f3d-4733-a042-c1e58bd15796.png)
 
 The data consists of following columns out of which we will be using the review star column in order to train our model as positive or negative based on whether if the review stars are 1 or 2 the it is regarded as 0(Negative) and if 3,4 or 5 star then it is regarded as 1(Positive).
![image](https://user-images.githubusercontent.com/70806075/179391410-24135dcd-5034-4cb8-bfcf-86929e18cb49.png)


TESTING THE MODEL:

⦁	The test data in the project has been given as a combination of Positive sentences related with joyful experiences and as Negative sentences related with failed product or poor experience of the recieved products.

It is always a good practice to train the model by using 80% or 70% of the dataset being used and then to use the remaining dataset for testing the same model.
The following division of the dataset for the purpose of training and testing the model is as shown below:

![image](https://user-images.githubusercontent.com/70806075/179391498-a020cee4-58a1-46d2-9988-b620fc205b99.png)
![image](https://user-images.githubusercontent.com/70806075/179391522-27735469-c250-4654-bd38-7095c5731499.png)

⦁	The dataset is uploaded to the repository along with code for ease and better understanding of the model.

Now it is the duty of this model to analyse these test values with respect to the model to understand the SENTIMENTS of the following values.
This is the entire concept of Sentiment Analysis Model.


OUTPUT:

The output of this model is hence expected to be on the basis of test values passed to the model wherein, 1 is for happy experience and 0 if for other test data according to which experience was not good.
![image](https://user-images.githubusercontent.com/70806075/179391680-d6026f30-30f3-4072-af7c-c2bfdd369367.png)

By the end of the model it is also equally important to calculate the accuracy of the model so as to recognise how well the model has been trained.
The accuracy of this model hence calculated is approximately 85.22%.
![image](https://user-images.githubusercontent.com/70806075/179391725-0dcba066-5c16-4432-84b8-06ffd4acf1d0.png)





