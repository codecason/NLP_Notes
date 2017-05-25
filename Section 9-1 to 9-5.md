### 9-1 Named Entity Recognition (NER)
  A very important sub-task: find and classify names in text:
Object, Person Name, 

### 9-2 Evaluation of Named Entity Recognition
  The extension of Precision, Recall, and the F measure to sequences.
 Boundary errors:
First Bank of Chicago announced earnings. // First was the first number of the sentence.
MUC scorer: 

### 9-3 Sequence Models for Named Entity Recognition
<br/>
  1.features for sequence labeling:
      words(words in dictionary)
      other kinds of inferred linguistic classfication
      label context
</br>
  2.Features:word substrings
      Example:
      drug, company, movie, place, person
        cotrimoxazole -- oxa,
        Wetherfield, -- field
        Alien Fury -- 
        Countdown to Invasion -- 
</br>
  3. Word shapes
      Varicella-zoster: Xx-xxx
      mRNA: xXXX
      CPA1: XXXd
      Comment:1，2，3 can be used for the features training.

### 9-4 Maximum Entropy Sequence Models
    1. Comment: Chars, words, phrases,lines and sentences are the parts of texts, what we 
    can do to divide them logically?
    Sequence problems
<br/>
    2. Conditional Markov Model (CMM) 
    Maximum Entropy Markov Model: MEMM,
        AIM: to predict the future appearing words in the sequence.
        divide texts to phrases--> give the phrases labels-->use optimization
        -->get the features of the current words-->label--> maximize the future 
        words
<br/>
    3.The probability prediction    
    REFER: Viterbi inference, Conditional Random Fields(CRF),
        Gradient Optimization
