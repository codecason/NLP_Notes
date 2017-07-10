### 17 Dependency Parsing

#### 17-1 Phrase Structure and Dependency Structure
1.
- The relation between of phrase structure and dependency
The head notion of a phrase(**dependency**)
2.
- Methods of Dependency Parsing
	- Dynamic Programming(like CKY algorithm) 
	- Graph Algorithms
		Maximum Spanning Tree (not minimum)

#### 17-2 Greedy Transition-Based Parsing
> MaltParser
1. Greedy discriminative 
2. Basic transition-based dependency parser
	The parsing process:
		3 parts: an input string, a set, a root ( = a stack)
		The parsing may not parse a phrase totally but in left-arc or right-arc mode, aside from shifting, reducing.
		Finish in the situation when β is null.
		e.g. right-arc : the head of a stack may take a right dependent word immediately
		The action are chosen by a discriminative (辨别) classifier.
3.  The classifier:
	- SVM, maxent
	Linear parsing
4. LPCFG (one best model)
5. The CoNLL-X(2006) shared task provides evaluation numbers for various dependency parsing approacheds over 13 languages.
6.	Problem:
	The dependency must be projective.
	

