# fake_news_detection
A machine learning project which classifies news as fake or real 

INTRODUCTION:

In our modern era where the internet is all over, everyone relies on various online resources for news. Along with the increase in the use of social media platforms like Facebook, Twitter, etc. news spread rapidly among millions of users within a very short span of time. The spread of fake news has far-reaching consequences like the creation of biased opinions to swaying election outcomes for the benefit of certain candidates. Moreover, spammers use appealing newsheadlines to generate revenue using advertisements via click-baits.

In this research work, the prime objective was to perform VARIOUS MACHINE LEARNING ALGORITHMS of various news articles available online with the help of concepts pertaining to Artificial Intelligence and Machine Learning.

Further, the aim of this work is to provide the user with the ability to classify the news as fake or real.



MOTIVATION:

There has been a rapid increase in the spread of fake news in the last decade, most prominently observed in the 2016 US elections. Such proliferation of sharing articles online that do not conform to facts has led to many problems not just limited to politics but covering various other domains such as sports, health, and also science. One such area affected by fake news is the financial markets, where a rumor can have disastrous consequences and may bring the market to a halt.
Our ability to take a decision relies mostly on the type of information we consume; our world view is shaped on the basis of information we digest. There is increasing evidence that consumers have reacted absurdly to news that later proved to be fake. One recent case is the spread of novel corona virus, where fake reports spread over the Internet about the origin, nature, and behavior of the virus. The situation worsened as more people read about the fake contents online. Identifying such news online is a daunting task.

Fortunately, there are a number of computational techniques that can be used to mark certain articles as fake on the basis of their textual content. There are a number of repositories maintained by researchers that contain lists of websites that are identified as ambiguous and fake. However, the problem with these resources is that human expertise is required to identify articles/websites as fake. More importantly, the fact checking websites contain articles from particular domains such as politics and are not generalized to identify fake news articles from multiple domains such as entertainment, sports, and technology.



METHODOLOGY USED:

In this project, we will be dealing with textual data.
We need to collect the news data, the data we are going to use is basically a labelled data set so it consists of several thousands of news articles and it will be labelled as either it is real news or fake news. 
The news data will consists of several details about the news such as author of that particular news, title of the news, text etc.
 
 ![image](https://github.com/divyaaxyz/fake_news_detection/assets/106904445/6d388d8d-d254-4c17-aab7-b375354d8444)


 
In this project, we will be dealing with textual data.
We need to collect the news data, the data we are going to use is basically a labelled data set so it consists of several thousands of news articles and it will be labelled as either it is a real news or a fake news. 
The news data will consists of several details about the news such as author of that particular news, title of the news, text etc.

Once we have this dataset we need to pre-process this data, a lot of work needs to be done in this pre-processing step, when compared to the numerical data because computers and systems do not understand text and characters, they just understand numbers so we need to find some suitable way to convert this text present in the news to meaningful numbers that the machine can understand. So we will perform various steps in this data pre-processing part.
For example, we will apply stop words function to our news data to filter out some high frequency words like articles, prepositions, pronouns, conjunctions, etc.  

We will also perform stemming in our data. Stemming is a natural language processing technique that lowers the infection in words to their root forms, hence aiding in pre-processing of text, words, and documents for text normalization. 
Next step in pre-processing is to convert the text into meaningful data that the computer can understand. This can be achieved by using Vectorization. The idea is to get the some distinct features out of the text for the model to train on, by converting text to numerical vectors which our computer/system can understand.

VECTORIZING DATA:
Vectorizing is the process of encoding text as integers i.e. numeric form to create feature vectors so that machine learning algorithms can understand our data.
 TF-IDF: It computes relative frequency that a word appears in a document compared to its frequency across all documents TF-IDF weight represents the relative importance of a term in the document and entire corpus . TF stands for Term Frequency: It calculates how frequently a term appears in a document. Since, every document size varies, a term may appear more in a long sized document that a short one. Thus, the length of the document often divides Term frequency.

IDF stands for Inverse Document Frequency: A word is not of much use if it is present in all the documents. Certain terms like ―”a”, ”an”, ”the”, ”on”, ”of” etc. appear many times in a document but are of little importance. IDF weighs down the importance of these terms and increase the importance of rare ones. The more the value of IDF, the more unique is the word.  TF-IDF is applied on the body text, so the relative count of each word in the sentences is stored in the document matrix. 
Once the pre-processing is done, we need to split the dataset into Training and Testing data wherein, most of the data is used for training, and a smaller portion of the data is used for mining.
This pre-processed data is now fed to our machine learning models .In this project, we will be using a number machine learning models which would be best suited for BINARY CLASSIFICATION. As this is a binary classification project which means we are going to classify the results into two types, it is either real or fake news. On training our machine learning models, we will get a trained model, we will do all our evaluations on this trained model.


