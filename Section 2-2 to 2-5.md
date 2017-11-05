### course 2-3 word tokenization
	fragment （语句）片段
	part of speech
	概念：token 一个词语实例
	命令行
		tr –sc ‘A-Za-z’ ‘\n’ < shakes.txt | sort |uniq –c | less
		tr –sc ‘A-Za-z’ ‘\n’ < shakes.txt | sort –n -r |uniq –c | less
		-c （count）
		不同语言的token划分怎么办？
		法语：L’ensemble: one token or two?
		word segmentation 分词？
		standard baseline segmentation algorithm （max matching）
			Doesn’t generally work in English.

### course 2-4
	Normalization 正则化
	Lemmatization 好像是归约？（归一）
	mophology 词语形态学
		stems
			Porter’s algorithm
				The most common English stemmer
		affix 词缀
		vowel 元音字母

### course 2-5
	SENTENCE SEGMENTATION
	punctuation
		!, ? are not ambigous
		. is quite ambigious
a decision tree to decide whether it’s a sentence’s end.
			implementing decision trees
				learned by machine learning
			SVM, Neural Networks, logistic regression.
