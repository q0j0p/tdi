As the branded food items database is unlabelled, latent topics were explored using Latent Dirichlet Allocation.  LDA  produces word groupings that represent topics that are derived using a generative model.  With the number of topics arbitrarily set to 10, the following results are obtained from the tokenized ingredients (limited to ten) in the Branded Foods database: 

|Topic | Words |
|:---|:---|
|Topic #0 | flour wheat niacin folic mononitrate riboflavin iron enriched oil acid |
|Topic #1 | organic rice seeds sunflower 100 honey brown cane pure coconut |
|Topic #2 | vitamin carbonated d3 palmitate milk natural fat water niacinamide flavor|
|Topic #3 | vinegar garlic salt oil pepper water tomato olive peppers spices|
|Topic #4 | acid corn citric potassium artificial syrup natural yellow red 40|
|Topic #5 | sodium salt chicken beef pork water powder contains corn dextrose|
|Topic #6 | organic juice concentrate water beans filtered apple ascorbic acid lemon|
|Topic #7 | cheese milk pasteurized enzymes salt culture cultured cream cultures skim|
|Topic #8 | tea orange almonds green spinach black pulp organic spring salmon|
|Topic #9 | milk cocoa sugar chocolate butter oil lecithin soy palm vanilla| 

On casual observation, the categories appear meaningful. Subjective labels were given based on the tokens chosen per topic.  Using cosine similarity with vectorized ingredients lists, food items closest to each topic was chosen: 

Topic | label | closest item 
|:---|:---|:---|
Topic 0 | baked goods |  MEIJER, ENRICHED ALL-PURPOSE FLOUR, cosine value: 0.858124389683 
Topic 1 | grain product (e.g. cereal, granolas)|  OUR DAILY EATS, CINNAMON CRANBERRY GRANOLA, cosine value: 0.517398389742
Topic 2 | non-sugar beverage | BORDEN, 2% REDUCED FAT MILK, cosine value: 0.521676947234
Topic 3 | sauces/soup (pasta sauce, chilli) | ARRABBIATA PASTA SAUCE, cosine value: 0.693238634307
Topic 4 | sugar beverage | Cherry Fountain & Shake Syrup, 1 gal jugs, UNPREPARED, cosine value: 0.846466960456
Topic 5 | meat | FAMOUS POLISH SAUSAGE, cosine value: 0.784302300308
Topic 6 | juices | HAPPY BABY, STARTING SOLIDS ORGANIC BABY FOOD, APPLES, cosine value: 0.647779953546
Topic 7 | processed dairy | RESER'S FINE FOODS, BAKED SCALLOPED POTATOES, cosine value: 0.662464155726
Topic 8 | natural foods | EARTHBOUND FARM ORGANIC, FLAVOR BLENDS SWEET KALE, cosine value: 0.461664098642
Topic 9 | sweets/desserts |  PEANUT BUTTER EGGS, cosine value: 0.768583121132

 
Although this is a qualitative evaluation, the proximity of the subjective guess to the closest food item indicates that results from LDA are coherent and can be meaningfully interpreted.  The method can be shaped in subsequent iterations to model healthy groupings of recipes.  
