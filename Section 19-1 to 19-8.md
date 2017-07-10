
### 19 Ranked IR
### 19-1 Introducing Ranked Retrieval
> There are many information retrieval models, one of which is Boolean search

> **These lectures can be seen in the book Introduction to Information Retrieval written by Chris Manning**

- Boolean search
ranked retrieval models
recollection
- Feast or famine: (too much or too little)not a problem in ranked retrieval
- Using query-document match

### 19-2 Scoring with the Jaccard Coefficient
#### Aim
Computing the similarity between documents

#### Problems
Not considering frequencies.

### 19-3 Term Frequency Weighting
##### Bag of words Model
The ordering of words in a document.
Log-frequency weighting
w(t,d) = 1 + log10(tf(t,d))

**score = SUM(w(t,d)) where t changes**

### 19-4 Inverted Document Frequency Weighting

> Which is tfidf, you can see it in Information Retrieval

idf(wi) = log(N / ni);
Where ni is the number of the documents that contains ni.
### Attention
idf doesn't affect the query of one-term query


### 19-5 TF-IDF Weighting
w(t,d) = (1+log tf(t,d)) * log(N / df(t))
Each document has a real-valued vector of weights of each word.


### 19-6 The Vector Space Model
|V|-dimensional vector space.
Formalizing vector space proximity and calculate the 
> The lecture shows a concrete process of computing tfidf and apply it to cosine measure.
#### The measure
1. Use angle instead of distance
2. From angles to cosines
3. L2 normalization (a measure in linear algebra)
    sqrt(L2 * L3) / (L2 * L3)
4. cosine similarity



### 19-7 Calculating TF-IDF Cosine Scores
Many search engines allow for different weightings:
	logarithmic tf or idf, cosine normalization
> This lecture shows a concrete example of querying using different cosine and tfidf.
#### Query progress
- each term t, -> fetch documents->
- calculate w(t,d) * w(t,q)
- return top K components.



### 19-8 Evaluating Search Engines
<h5> Introduction
- How fast
- precision / recall / f measure (basic concepts in IR)
- mean average precision
