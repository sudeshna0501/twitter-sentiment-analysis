# twitter-sentiment-analysis
 Sentiment analysis is, basically, 
a text classification method that helps in identifying whether an online writing carries a 
positive, negative, or neutral connotation to it. Sentiment analysis finds its significance in a 
lot of domains these days, the most popular among them being brand and social media 
monitoring. Most businesses are mindful of their customers’ opinions on their products, 
thereby working on their strengths, and enhancing customer experience, which in turn, 
benefits them. It even helps in finance and stock monitoring with the correct analysis of 
customer sentiments for a more beneficial investment into it. 

The purpose of the research is to figure out whether a tweet in English language is favorable, 
negative, or neutral. The strategies in this case are: (1) a few deep learning-based techniques, and (2) a hybrid approach. For the deep learning methods, a Multichannel CNN method, a combination of LSTM and CNN algorithm have been implemented. BERT in combination with other deep learning algorithms have also been used. Among the lexicon-based approaches, a polarity dictionary in combination with BERT have been used to 
get good results on the approach.

**(1)Deep Learning Based Approaches**
  ---MULTICHANNEL CNN

The entire process consists of data preparation and developing the model. For 
data preparation, the sentiment part of the raw data is encoded using a label encoder and 
converted to categorical values, while the tweets are loaded and cleaned to remove 
punctuations, numerical, stop words and other irrelevant characters.

