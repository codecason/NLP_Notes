## Relation Extraction
### 10-1 Extracting relations from text
		1. relation extraction’s use
			create new structured knowledged bases
		2. Automated Content Extraction (ACE)
			some kinds of relation combination
		3.Relations databases drawing from Wikipedia
			DBPedia: 1 billion RDF triples, 385 from English Wikipedia
		4.Ontological relations
		5.How to build extractors
			Supervised Learning
			Using patterns

### 10-2 Using Patterns to Extraction Relations
		1. Hearst’s Patterns for extracting relations
			i.e: X and other Y
		2.Some Richer Relations Using Rules
			Pattern: ORG-LOC, PER-ORG, DRUG-DISEASE
		3.Named entities are not enough for the relations
			some relations are different between same entities

### 10-3 Supervised Relation Extraction
		1.Supervised Learing
			1)choose relations
			2)choose a set of named entities
			3)choose a representative corpus
			label the named entities in the corpus
			hand-label the relations between these entities
			break into training, development and test
		2.Word features
			M1, M2 ‘s relation:
			M1, M2’s headwords,bigram, type, level(noun)
			NP(noun phrase), VP, PP...

### 10-4 Semi-Supervised Relation Extraction
		1.relation bootstrapping(Hearst 1992)
		seed
		2.Snowball
		3.distant supervision
			combine bottstrapping with supervised learning
		4.Distantly supervised learning of relation extraction patterns
			1)For each relation i.e. born-in
			2)For each tuple in big database <Elbert, Hubble>
			3)Find sentences in large corpus
			4)Extract frequent features (and later can be used by parsers)
>Tip:DBPedia
