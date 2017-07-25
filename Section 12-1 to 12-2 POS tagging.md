## POS Tagging
###		12-1 An Intro to Parts of Speech and POS Tagging
The concepts of parts of speech->noun, verb, adv, prep, conj, pron...
particles: off, up
open class (lexical)words + closed classes

**POS**: part of speech
    The problem of ambiguity in POS Tagging: regexps, text-to-speech
Some appendixes:
-   CC - Coordinating conjunction
-	CD - Cardinal number
-	DT - Determiner
-	EX - Existential there
-	FW -Foreign word
-	IN - Preposition or subordinating conjunction
-	JJ - Adjective
-	JJR - Adjective, comparative
-	JJS - Adjective, superlative
-	LS - List item marker
-	MD - Modal
-	NN - Noun, singular or mass
-	NNS - Noun, plural
-	NNP - Proper noun, singular
-	NNPS - Proper noun, plural
-	PDT - Predeterminer
-	POS - Possessive ending
-	PRP - Personal pronoun
-	PRP$ - Possessive pronoun
-	RB - Adverb
-	RBR - Adverb, comparative
-	RBS - Adverb, superlative
-	RP - Particle
-	SYM - Symbol
-	TO - to
-	UH - Interjection
-	VB - Verb, base form
-	VBD - Verb, past tense
-	VBG - Verb, gerund or present participle
-	VBN - Verb, past participle
-	VBP - Verb, non-3rd person singular present
-	VBZ - Verb, 3rd person singular present
-	WDT - Wh-determiner
-	WP - Wh-pronoun
-	WP$ - Possessive wh-pronoun
-	WRB - Wh-adverb
Deciding on the correct part of speech can be difficult even for people.
Experiment: In the Brown corpus, 40% of the words are ambigious.


### 12-2 Some Methods and Results on Sequence Models for POS Tagging
What are the main sources of information for POS tagging? Generally, we think that 
the neighbour words are, but in fact, it isn’t.
		Continuing above, it can be suprisingly well if we check it the word in its own.
		POS Tagging Accuracies:Trigram 
Trigram HMM -95% / -55%
		Maxent P(t|w): 93.7% / 82.6%
	Using words only in a straight classifier works as well as a basic sequence model(HMM), which is out of expectation.
