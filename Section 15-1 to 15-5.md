## 15 Parsing
### 15-1 CFG and PCFG
>CFG:Context-Free Grammar
>PCGG: Probabilistic Context Free Grammar

#### CFG:
- Phrase structure grammar
- use G as a grammar, G = {T, C, N, S, L, R}
- C: preterminals (What's this?)
- T: terminals
- N: non-terminals
- L: Lexicon 
- R:Grammar

#### PCFG:
- add a probability after each rule
- e.g. N->people 0.1

### 15-2 Grammar Transforms
>Aim: restricting a grammar to CNF can improve parsing effeciency, though it's not always possible.

>In computer science, a context-free grammar is said to be in Chomsky normal form if all of its production rules are of the form:
A -> BC, or
A -> α, or
S -> ε

#### 1.Chomsky Normal Form
>e.g.
>To reduce the existing rules in a grammar.
>S->NP VP
>VP->V NP
>NP->NP (delete)
>P->P (delete)

#### 2. Binarization in Chomsky Normal Form
>1.Cubic time of PCG parsing.
2.Treebank: empties and unaries
	

### 15-3 Cocke-Kasami-Younger (CKY)

#### 1.Constituency Parsing
In the given input of sentences, try to find out the most likely meaning(parsing).
**Viterbi(Max) Scores** (This may be used in HMM model)
#### 2.Extended CKY Parsing
- Unaries can be incorporated into the algorithm.
People fish tanks
#### 3. CKY Algorithm
- or known as CYK algorithm
- [The CYK Algorithm - Wikipedia](https://en.wikipedia.org/wiki/CYK_algorithm)
> The algorithm requires the context-free grammar to be rendered into Chomsky normal form (CNF), because it tests for possibilities to split the current sequence in half. 

### 15-4 CKY Parsing Example

- 1 First, A triangle like probability matrix
- 2 Second, fill the matrix with the rules and the probability.(The y values are the words)
> like this: N->fish 0.2 to fill score\[0\]\[1\]

- Fill process:
- First, the diagonal.
- Second, combine the constituents(???).
- Update the score and mark back(of the process of parsing).
- Last, call the function buildTree(score, back) to get the best parsing.

### 15-5 Evaluating constituency
Constituency Parser Evaluation

> Using brackets to represent the tagging.

- Label Precision
- Label Recall
- Parsing accuracy: LP / LR F1
- Tagging accuracy
