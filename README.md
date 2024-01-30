# Language-Processing-with-Python
This is a sentiment analysis work using keras and python. I'll train machine learning models to classify IMDB moview reviews into positive or negative category. 

#### Dataset
The dataset contains IMBD movie reviews and is available to download from this link:  http://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz

It contains 50,000 movie reviews with equal number of instances for the positive and negative labels.

#### Preparing text data
In a typical workflow, text data processing requires the following steps:
- tokenization
    - split into smaller units e.g., words or characters
- standardization
    - convert all text to lowercase, remove punctuation, stopwords etc.
- convert tokens to numeric representation
    - index the tokens
    - map tokens to numeric vector

Since these tasks are very common, there are already a number of builtin libraries in Python. I have used sklearn and keras to handle the text preprocessing part.

#### Defining the model
There are two types of model considering the order of the words:
- Bag-of-words model: discard word order
- Sequence model: carry information about word order

Here I have used the bag-of-words approach. It is generally a good idea to start with a simpler model and gradually go for more complex models. In the first notebook, I have established a baseline using LogisticRegression model. Then I experiemnted with n-gram models as it keeps a small amount of local word ordering. Since the data is balanced, I have used "accuracy" as the evaluation metrics.
