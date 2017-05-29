## 16 Parsing of PCFG
### 16-1 Lexicalization of PCFGs
> PCFG: probabilistic CFG
> Magerman 1995, Collins, Charniak 

- **Estimators of a phrase's structure and meaning**
- Draw a tree where each subtree(with 3 nodes) is corresponding to a rule
- We can calculate the probability in order to decide whether a given word should be ahead of another word in the sentence, and hence get the structure

#### Conclusion
- Word-to-word affinities are useful for certain ambiguities

### 16-2 Charniak's Model
> In 1997, by Charniak
> A straight forward method to parse PCFG

#### Details
- The probability of verbal complement frames
Bilexical probabilities
> P(prices | n-plural) = .013
> P(prices | n-plural, NP) = .013
> P(h|ph, c, pc)
> linear interpolation shrinkage 

- problem
> when using Maximum Likelihood Estimate, people may commonly sees previously unseen events, which would have probability 0.

### 16-3 PCFG Independece Assumptions
> the independence assumtions may be too strong(and hence make the parsing result unprecise)
 
#### Refining the grammar 
Johnson 98
- using state splitting and encode the symbols, like NP to NPs
- parent annotation
- marking possessive NPs (only in English)

### 16-4 The Return of Unlexicalized PCFGs
1. A much better way than lexical PCFG;
2. what "unlexicalized" PCFG mean:
	Grammar rules are **not systematically specified**
3. experimental approach
#### Horizontal Markovization
Merge states
#### Vertical Markovization
rewrites depend on past k ancestor nodes(in parse tree)
#### Unary Splits, Tag Splits, Yield Splits
#### Distance / Recursion Splits

<br></br>
### 16-5 Latent Variable(隐含变量) PCFGs
>Petrov and Klein 2006, 2007
When there is some situations that cannot be tagged directly from sentences, we should take care of the method of HMM to calculate latent variables.
#### Learning Latent Annotations(隐含标签)
Using EM algorithms, like Forward-Backword for HMMs, but constrained by tree.
#### POS tag split based on the method of semantic classes
