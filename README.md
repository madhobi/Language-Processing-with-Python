# Language-Processing-with-Python
This is a sentiment analysis work using keras and python. The dataset contains IMBD movie reviews and is publicly available to download from this link:  http://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz. I'll train machine learning models to classify the reviews into positive or negative category. 

#### Preparing text data
In a typical workflow, text data processing requires the following steps:
- tokenization
    - split into smaller units e.g., words or characters
- standardization
    - convert all text to lowercase, remove punctuation, stopwords etc.
- convert tokens to numeric representation
    - index the tokens
    - map tokens to numeric vector

#### Two types of model considering word order
- Bag-of-words model: discard word order, ususally uses n-gram tokenization as it keeps a small amount of local word ordering
- Sequence model: care about word order, usually uses word-level tokenization
