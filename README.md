Sentiment-Analysis

INTRODUCTION:

It is a project based on NATURAL LANGUAGE PROCESSING(NLP) that deals with devlopment of various applications that can be used by machine to decode the Human Language.

NLP can be defined as the process of translating Textual data into meaningful data.

NLP uses the NATURAL LANGUAGE TOOL KIT(NLTK) which is a very powerful NLP library that consists of packages that help machine understand the human language.

There are basic three processes involved in NLP.

⦁	The first process is related with DATA CLEANING.
	Data cleaning consists of multiple steps such as Tokenization,Stop word removal,Stemming and Lemmatization.
  
⦁	The second process deals with VECTORIZATION.

⦁	The third process is related with DATA CLASSIFICATION.
  Data classification is known as text tagging or text categorization.


PROCESS:

1.DATA CLEANING: Cleaning the raw data.

⦁	TOKENIZATION is defined as the process of dividing the entire document or paragraph into smaller units of individual words or phrases. These smaller units are called Tokens.

⦁	STOP WORD REMOVAL is the process of removing those words or phrases whose presence has no effect on the overall analysis of the data.

⦁	STEMMING is the process of converting the words to its roots.The project uses the PORTER Stemming process for the purpose of stemming.

2. VECTORIZATION: Mapping of words or phrases to a vector of real numbers.

3.DATA CLASSIFICATION: Categorizing the data into individual groups.
  Data Classification is based on the NAIVE BAYES ALGORITHM


NAIVE BAYES ALGORITHM:

Naive bayes algorithm is based on the Bayes theorom of mathematics that deals with the Conditional Probability of the data.
According to Naive Bayes algo, "Probability of event A to occur when B has already occured is equal to the product of Posterior probability and Prior Probability"


LIBRARIES USED:

⦁	Tokenization process uses the "RegexpTokenize" library of "nltk.tokenize" package.

⦁	Stop word removal technique uses the "StopWords" library of the "nltk.corpus" package.

⦁	For stemming the project uses the PORTER STEMMER METHOD.
  
  It uses the "PorterStemmer" library of the "nltk.stem.porter" package.
  
![image](https://user-images.githubusercontent.com/70806075/177722870-9777e492-fa2f-43ad-aeee-669c9ce8e2de.png)


⦁	Vectorization uses the "CountVectorizer" library of the "sklearn.feature_extraction.text" package.
![image](https://user-images.githubusercontent.com/70806075/177723917-2d6335b8-5cc5-414f-94e6-74878db23109.png)

⦁	.For Classification purpose the project uses the MULTINOMIAL NAIVE BAYES algorithm.
  
  It uses the "MultinomialNB" library of the "sklearn.naive_bayes" package.
![image](https://user-images.githubusercontent.com/70806075/177724147-9257ab15-c377-46a3-a2cf-eba4eea81b52.png)

TRAINING THE MODEL:

The project uses a train data so as to train the model. This train data consists of several sentences that are feeded to the system so that they can be recognised as sentiments of positivity or negativity.

This data set is used to help machine understand the basic words which are used by each and every individual to share his feelings.

Based on this , the constraints for the data are given according to which 1 is for Positive textual data and 0 is for Negative textual data.

![image](https://user-images.githubusercontent.com/70806075/177722633-a6102fb3-0bc7-400b-9d09-1ef833728571.png)

TESTING THE MODEL:

⦁	The test data in the project has been given as one Positive sentence related with "happiness,enjoyment,etc. ,other joyful intentions".

⦁	The second test data has been given as a Negative sentence related with "sadness,crying,etc. other bad experiences".
![image](https://user-images.githubusercontent.com/70806075/177723800-eb3e479c-cf55-4428-aa80-3f3c5be62234.png)

Now it is the duty of this model to analyse these test values to understand the SENTIMENTS of the following values.
This is the entire concept of Sentiment Analysis Model.


OUTPUT:

The output of this model is hence expected to be [1,0] on the basis of test values passed to the model wherein, 1 is for happy movie experience and 0 if for other test data according to which movie experience was not good.
![image](https://user-images.githubusercontent.com/70806075/177724250-e8611b15-1159-4ada-91ee-0fb93807c588.png)



