NMF is the factorization of a matrix (say, V) into two matrices (W and H) with the condition that they are composed of non-negative elements.  The decomposed matrices provide useful properties: reduction in dimensions that can be efficient approximations of the original; “clustering” of elements into latent topics when factorized to minimize error (||V-W||^2); imposing non-negativity condition on elements makes values easier to interpret.  It is a numerical approximation that can be solved with different algorithms (namely, alternating least squares, multiplicate factorization).  

### Dimensions of matrices
Given V: m x n, W is m x k, while H is k x n.  
k is the main hyperparameter to designate dimensionality(# of topics). 


### NMF applied to recipe ingredients, processed as document terms a la NLP  
#### [Deriving topics from recipe ingredients](https://github.com/q0j0p/food/blob/master/src/model/topic_model_recipes_NMF.ipynb)