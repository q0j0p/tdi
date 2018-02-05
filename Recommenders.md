Focusing on utility that is appropriate to the task, a few recommender types can be explored: 
- content-based filtering (e.g. ingredients) 
- collaborative filtering (based on user preferences and item similarity) with matrix factorization 
- graph based 

### Topic modeling, dimensionality reduction, clustering
These three related concepts are fundamental to many aspects of machine learning.  

- Clustering is most relevant to content-based filtering in that documents are grouped according to similarity.  
- Dimensionality reduction strives to derive a smaller set of features while maximizing the distinguishable characteristics in a dataset with the use of matrix factorization. 
- Topic modeling is a combination of soft clustering and dimension reduction to come up with meaningful groupings; each document is assigned a distribution of topics with different weights.  

In the context of the current dataset where I have a collection of recipes with an ingredients list, directions, images and a related collection of member reviews and ratings plus implicit feedback and social connections, several analyses are possible.  

## [User similarity based on recipe ingredients](https://github.com/q0j0p/food/blob/master/src/model/model_member_similiarity.ipynb)
## [Recipe recommendation based on content (similarity of ingredients in made recipes)](https://github.com/q0j0p/food/blob/master/src/model/model_content_similarity.ipynb)