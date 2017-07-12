## Advanced Maxent
### 11-1 The Maximum Entropy Model Presentation
		Also named maxent.
		The examples of entropy when two probabilities(ph and pt) change.
    And the aim is to maximize the entropy of the probability(as extracted from the problem).
		The convexity of the function(only an introduction).
		H(p) = -∑xlogx is convex(in the domain of xi).
    
### 11-2 Feature Overlap_Feature Interaction
		Unlike NB Model, the Maxent model doesn’t count double.
    Feature interaction is a software engineering concept. 
    It occurs when the integration of two features would modify the behavior of one or both features.
    Due to the calculating complexity, only used for models with small count of features(4-8).
    
### 11-3 Conditional Maxent Models for Classfication
		In the space of CXD as a complex X, C is a generally small.
		In principle, build models over P(C,D).
		C is small, D marginal may be huge.
			Expectation of features over CXD. E(fi) = sum(P(c,d)fi(c,d))

### 11-4 Smoothing-Regularization_Priors
	Issues: Maxent models have well over a million features.Even storing a single array 
  of parameter values can have a substantial memory cost.
  Given a Empirical distribution(like a PDF function), calculate its likelihood like
  logP(h,t|λ)(with freedom-degree λ and vars h and t), try to draw a picture of the distribution
	The issue: early stopping.
		Smoothing: Priors-> Gaussian Priors->derivative
		->An example:POS Tagging
		->Smoothing helps:
			softens distributions, expananatory features, speeds up convergence.
