# Hate_Speech_Classification
Hate speech classification in three various approaches: Tfidf SVM, Word level CNN, and Character level CNN
The dataset used is the combination of 3 seperate datasets: 
Kaggle's toxic comment dataset: https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data;
Kaggle's tweeter hate speech dataset: https://www.kaggle.com/vkrahul/twitter-hate-speech/version/1;
Aitor-garcia-p's hate speech dataset: https://github.com/aitor-garcia-p/hate-speech-dataset
The total amount of entries are around 200k, and the positive entries(hate speeches) are around 20k. With this amount of data, it is hard to tell before hand whether machine learning or deep learning approach would perform better, so I trid both ways.
Turns out word level CNN has the best result: precision -- 95% , recall -- 94%
Tfidf SVM is slightly less than word level CNN: precision -- 94% , recall -- 93%
And Character level CNN has the lowest score of the three: precision -- 93% , recall -- 93%
It is also worth metioning that the training time for SVM is considerably longer than the other two, it took around 1.5 hours for SVM to go through the training set, while it took only minutes for the deep learning approaches.

Here's a graph of the most used words in hate speeches and neutral comments:
![alt text](https://github.com/WeiLiu6/Hate_Speech_Classification/blob/master/images/Word_Freq.jpg)
