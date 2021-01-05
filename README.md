# Recipe search engine

## Overview
Unlike the regular search engines, recipe search engine needs an unconventional approach.

There are some categories in recipe searching, such as 'ingredients', 'tools', and 'cooking time'.

By using NLP POS-Taging method, it extracts keywords from the search query.

Then, it classify each keywords and store them into category accordingly.

These keywords would be used as score or filter.

The ‘Latent Dirichlet Allocation’ method is used to create an additional category. It is useful to filter out the irrelevant recipe.

Build ranking function based on the importance of each categories.

## Dataset

The dataset is present on Kaggle produced by Elisa. 

https://www.kaggle.com/elisaxxygao/foodrecsysv1

The dataset was constructed via collecting Allrecipe.com recipe data. 

The data is a collection of recipes posted between 2000 and 2018. 

49698 recipes are present in total. 

Columns : recipe_id , recipe_name, aver_rate, image_url, review_nums, ingredients, cooking_directions, nutritions, and reviews. 

The cooking direction column contains cooking time, and nutritions column contains the amount of following nutritions :  calories, sugars, caloriesFromFat, calcium, sodium, folate, fiber, thiamin, magnesium, iron, potassium, saturatedFat, cholesterol, vitaminC, carbohydrates, fat, niacin, vitaminA, vitaminB6, protein.
