## 21 Question Answering
### 21-1 What is Question Answering
Examples:
- Waston
- Wolfram Alpha

IR-based QA
**Problems:**
- question processing
- passage retrieval
- answer processing


Knowledge-based QA
- Siri (build a semantic representation of the query)

### 21-2 Answer Types and Query Formulation
**Question Processing**
- Answer Type Detection
- Query Formulation
- Question Type classification

1.**Answer Type Taxonomy**
Just like tagging answers.
2.**Answer Type Detection**
Some rules to find answer type
3.**Keyword Selection Algorithm**

### 21-3 Passage Retrieval and Answer Extraction
Features for Passage Ranking
- named entities, query words, N-grams, proximity, longest sequence of question words

Using Machine Learning:
- Features for ranking.

Common Evaluation Metrics
- Accuracy
- 
#### Summary
When you do NLP works, you may find it hard to judge the quality of your method and its drawbacks, so you need better look for some evaluation work.But the evaluation measure also need reasonable support.You can try to find the answers in essays, articles, but you must be critical about what you read.
However, doing is better than reading.Just do it and find how good it is.

### 21-4 Using Knowledge in QA
**Relation Extraction**
	Like a table in a relation database
**Temporal Reasoning**
	Time sequence judging
**Geospatial knowledge**
	Like some locations
**Context and Conversation**
	Coreference helps resolve ambiguities.
	(like some context-based conversation in dialogues.)

### 21-5 Advanced_Answering Complex Questions
- i.e. Q:What is water spinach?
- i.e. Q: **some other more complex questions**

**The Architecture**:
Document Retrieval->Predicate Identificatin->Data driven analysis->Definition Creation
