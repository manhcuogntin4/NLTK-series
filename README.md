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
The map phase of MapReduce consists of mapping splits of the input data to key-value pairs


MapReduce offers a robust and conceptually simple framework for implementing index  construction  in a distributed environment

Dynamic indexing:
But most collections are modified frequently with documents being added, deleted, and updated.  This means that new terms need to be added
to the dictionary, and postings lists need to be updated for existing terms

If there is a requirement that new documents be included quickly, one solu-tion is to maintain two indexes: a large main index and a small
auxiliary index that stores new documents.  The auxiliary index is kept in memory. Searches are run across both indexes and results merged. Deletions are stored in an invalidation bit vector. We can then filter out deleted documents before returning the search result.   Documents are updated by deleting and reinserting them. Each time the auxiliary index becomes too large, we merge it into the main index.


