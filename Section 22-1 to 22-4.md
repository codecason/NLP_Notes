## 22 Summarization(not of the course)
### 22-1 Introduction

- Single-document
- Multiple-document
- Generic-document
- Summarization for Question Answering:
	Snippets
- Extractive Summarization
- Abstractive Summarization
**Evaluation**
BaseLine: The first sentence

### 22-2 Generating Snippets
Basic Summarization Algorithm:
1.Content selection
	Unsupervised Content Selection (1958)
	Supervised Content Selection: Labeled
2.Information ordering
3.Sentence realization

### 22-3 Evaluating Summaries
I.
**ROUGE**:Recall Oriented Understudy for Gisting Evaluation

II.
**Get instrinsic (:authentic, real) metric**
Input a D, and an automatic summary X:
	Output: An evaluation
	**ROUGE** ________
	Principle: Compare it with human summaries.

### 22-4 Summarizing Multiple Documents
>flow-chart of summarizing multiple documents
Maximal Marginal Relevance(MMR)

LLR+MMR
1.Score each sentence based on LLR.
2.Include the sentence with highest score.
3.Iteratively add into the summary.

**Domain-specified Knowledge**