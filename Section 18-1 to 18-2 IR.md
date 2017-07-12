## 18 Information Retrieval
> The content could be found in the course of Information Retrieval, so this part could be ommited.

### 18-1 The introduction to information retrieval
1. Unstructured text vs. structured data(database).
2. The classical Search Model
	User task->info need->query->**search engine**<-collection
	Search Engine->results->query refinement->query->(loop back)
3. Precision and callback.
	
### 18-2 Term-document Incidence Matrices
Shakespeare's representations.

### 18-3 Inverted-Index
> You can find it in some course of search engine.
- Tokenization
- Nomarlization
- Stemming
- Stop words


### 18-4 Query Processing with the inverted index
 
 Use merge sort to merge two posting lists.(based on the number of some kind of evaluation)
 
### 18-5 Phrase Queries

> something like advanced search
 Problems
 - implicit phrase queries
 Solution Attempt
 - Biword indexes (cost too much space)
 - Positional indexes (document merge algorithm, also too large)
 - combination schemes
