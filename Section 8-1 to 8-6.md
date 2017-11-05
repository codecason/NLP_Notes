### 8.1 Generative vs. Discriminative Models
    generative model：a joint model of conditional(discriminative) model and Markov model
    Bayes Net/Graphical Models
    Joint Likelihood：联合相似度
    conditional model:条件模型
    Even with the same features，changing from the joint models to conditional models improves the performance.

### 8.2 Making features from text for discriminative NLP models
    特征：判断语言中符合某个特征的判断器
    empirical ：多个特征判断函数的结果求和
    Feature-Based Model
    Feature-Selection:特征选择 Zhang and Oles （2001）Text Categorization
    Naive Bayes（generative model） 和其他discriminative模型相差很大，但是discriminative模型之间差距很小
    Tip: 数据集classic reuters data set

### 8-3 Feature-Based Linear Classfier
classfication：
	using linear classfiers to classify the classes
	lambda i is the weight, fi is a function, c is a class, d is a observation of 
	d which makes  vote(c) ∑λ(i)fi(c,d) maximal.
	later calculate the conditional likelihood of：P(c|d,lambda)
perceptron
	2)
	Logistic regression
	maxent models (essentially the same as multiclass logistic regression models)
	maxent: max entropy
	feature functions
	building a maxent model:

### 8-5 Generative vs. Discriminative models
	The problem of overcounting evidence, when facing relative variables.

### 8-6 Maximizing the likelihood
	enumerator dominator
	
#### the log likelihood
	finding the parameter to minimize the log conditional likelihood
