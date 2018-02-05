## Allrecipes website data

Recipe and member pages (examples below) were scraped using both a local machine and AWS EC2 instances and stored in an S3 bucket.  

<img src="https://github.com/q0j0p/food/blob/master/notes/resources/shorecook.png" width="300">


<img src="https://github.com/q0j0p/food/blob/master/notes/resources/recipe2.png" width="300">



To get a diverse yet structured sampling of the entire network, I first scraped the ["ask the community"](http://dish.allrecipes.com/ask-the-community/), which is a Q&A forum where members interact with questions and comments about anything from cooking methods to website configuration.  This resulted in ~ 1000 unique member IDs.  Subsequently, their member page (which is a collection of 6 pages: "about me", "favorites", "reviews", "personals" "followers", "following") were all scraped and stored. 

[Summary notebook of allrecipes database](organize_allrecipes_db.ipynb)

## USDA Data
Data for food items were obtained via API from the [USDA food composition database](https://ndb.nal.usda.gov/ndb/search/list).

* [Summary of `usda_db`](organize_usda_db.ipynb)
