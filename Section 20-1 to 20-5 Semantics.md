## 20 Semantics
### 20-1 Word senses and word relations
Reminder: lemma and wordform
lemma
#### homonymy
same sound and different meaning
- Information retrieval
- Machine Translation
- Text-to-speech

#### polysemy
A systematic relationship between senses
Lots of types of polysemy are systematic
School, university, hospital

#### synonymy
same meaning relationship

### antonyms
reverse meaning.

- hyponymy (like subclass)
- hypernymy (like hyper class)
hyponymy is usually transitive (A->B, B-> => A->C)

### 20-2 WordNet and Other Online Thesauri

synset: synonym set
#### Relation
hypernym
hyponym
member meronym
#### WordNet
- [WordNet Page](http://wordnetweb.princeton.edu/perl/webwn)
- Mesh Hierarchy
Ontology

### 20-3 Word Similarity and Thesaurus Methods
> The methods can be summarized as thesaurus-based methods.

####Synonymy

#### Similarity
**1.Path based similarity**=>Two concepts are similar if they are near each other in the thesaurus (or the tree)

**2.Refinements to the similarity: **
simpath(c1,c2), wordsim(w1,w2)=max sim(c1,c2)

##### 3.Information content similarity metrics
3.1 Resnik(Not resink) Method
3.2 Dekang Lin method, 1998. ICML=>
	2log(LCS(c1,c2)) / (logP(c1) + logP(c2))
3.3 The Lesk Algorithm

### 20-4 Word Meaning and Similarity I
**Distributional Similarity**
>problems with 20-3=> recall is bad, not applicable to every language.

**Term-context matrix**
=>
1. word vectors
2. Context vectors
3. Pointwise mutal information
4. PMI is biased toward infrequent events

### 20-5 Word Meaning and Similarity II
**Using syntax to define a word's context**
Once you have PPMI matrix, you can compute=>
**Cosine as a similarity metric**
