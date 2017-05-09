# NLTK-3----Natural-Language-Processing-with-Python-series
Natural Language Processing with Python 3 and NLTK 3 series
http://pythonprogramming.net/tokenizing-words-sentences-nltk-tutorial/

1: Some term in nltk

Corpus: a text part of document

Tokenization : Convert corpus to line or words

Stop word: extremly common words can be remove 

Normalisation: looking for the words of same meaning : USA, U.S.A, automobile car, convert text to miniscule.. remove Accents and diacritics: 
cliché -> cliche, naîve->naive

Stemming and lemmatization :
am, are, is ⇒ be
car, cars, car’s, cars’ ⇒ car

2: boolean queries

The doc is convert to index
word->list of page that containt words
Index can be organized in the tree (binary tree ) for searching :
Some technique for queries
General wildcast query

3:Technique for correct spelling:
3.a Isolate ternm correct spelling
Edit distance : Levenshtein distance (number of edit insert, delete, replace)
k-grams indexes
3.b Context sensitive correct spelling

4: Indexing
4a Some concept
Token
Term
Posting list: a list of torken id and the document id
Two algorithms for indexing (local)
blocked sort-based indexing algorithm BSBI
single-pass in-memory indexing or SPIMI

Distributed indexing
MapReduce, a general architecture for distributed computing

