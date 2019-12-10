# Word2Vec-from-Philippine-Tweets
A word2vec model trained from tweets collected within the Philippines from 2016

As there is a lack of available NLP resources for minor languages such as Filipino, Bisaya, etc. online, I’m sharing the word embedding model I trained for my [study](http://pejard.slu.edu.ph/vol.9/2019.10.01.pdf) using Gensim’s implementation of word2vec. This model was designed to implement transfer learning, allowing development of improved machine learning models over Philippine social media datasets. The model was trained from tweets posted within the Philippines from year 2016. It contains 374,118 words each represented with a 50-dimension vector. 

You can download the word2vec model [here](https://drive.google.com/open?id=1ZhbtTBRmkR6SOMajTkOpdD2YhQ4hKcw7).

And [here](http://pejard.slu.edu.ph/vol.9/2019.10.01.pdf) is the paper detailing the development of the word2vec model:
```
Marges, A.T. and Samaniego, J.M. (2019). Philippine e-Journal for Applied Research and Development 9(2019), 27-39.
```

## Usage
You’ll need the Gensim module. Then, to load the model:
```python
>>> from gensim.models import Word2Vec
>>> model = Word2Vec.load("phil_tweet.w2v")
```
You can refer [here](https://radimrehurek.com/gensim/models/word2vec.html) for more details on how to use the pretrained word2vec model.
