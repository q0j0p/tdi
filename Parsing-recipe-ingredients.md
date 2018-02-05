Allrecipes is an extensive collection of ingredients contributed by users.  Hence, most of the data are free form, and data cleanup can be a challenge.  

### Parsing recipe ingredients 
[This article](https://open.blogs.nytimes.com/2015/04/09/extracting-structured-data-from-recipes-using-conditional-random-fields/) describes how the New York Times has tackled the inconsistencies of ingredients lists. 

My preliminary parser turns each ingredient string into a list of: 
quantity (float), unit (string), ingredient term (list of tokens).  
- [Parsing recipe ingredients](https://github.com/q0j0p/food/blob/master/src/data/allrecipes/parse_recipe_ingredients.ipynb)