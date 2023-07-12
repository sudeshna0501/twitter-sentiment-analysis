# twitter-sentiment-analysis

The purpose of the research is to figure out whether a tweet in English language is favorable, 
negative, or neutral. The strategies in this case are: (1) a few deep learning-based techniques, and (2) a hybrid approach. For the deep learning methods, a Multichannel CNN method, a combination of LSTM and CNN algorithm have been implemented. BERT in combination with other deep learning algorithms have also been used. Among the lexicon-based approaches, a polarity dictionary in combination with BERT have been used to 
get good results on the approach.

**(1)Deep Learning Based Approaches**
  ---MULTICHANNEL CNN

The kernel size is modified according to the n gram sizes used as input. The entire process consists of data preprocessing and model development. An Embedding layer generated from a tokenizer is used as the input of a conventional model for document classification, followed by a one-dimensional convolutional neural network, a pooling layer, and finally a prediction output 
layer.

--LSTM + CNN

The basic idea behind this model is also similar to the multichannel CNN, but for LSTM, a character-level tokenization is done, while for CNN, a word-level tokenized layer is passed, with two channels of different kernel sizes.

--BERT

For BERT, a sentence bert model is used for the particular script as well as for subsequent scripts combining BERT with other models, in order to get the embeddings for it. These embeddings are passed through a few dense layers eventually to obtain the final score.

--BERT + BILSTM

The same sentence embeddings obtained from BERT were passed along with the output from a dense and concatenated together to perform the classification operation.

**(2)Hybrid Approach**
--BERT + LEXICON + CNN

The data is divided by a 1:1 ratio. One-half of the dataset is passed through BERT model to find out the sentence embeddings. The rest is tokenized, and a matching algorithm is used to find out the number of words that match with the polarity wordnet. A vector is created that contains the sum of positive tweet words found in the 30wordnet list and a sum of the negative tweet words in the corresponding wordnet list. Both the BERT embeddings and the lexicon vectors are passed through a dense layer, concatenated and then passed through a softmax layer to finally obtain the output layer.


**DATASET USED:**
The dataset used was:  US airline twitter dataset (available on Kaggle)

The lexicons have been uploaded in this repository.

