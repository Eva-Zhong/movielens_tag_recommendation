# About this project

In this project, I applied a few natural language processing algorithms to identify which tags that users of movielens--a movie recommendation website--applied best characterize these movies. 

Movielens is a movie-recommendation website mainted by GroupLens, University of Minnesota. Data gathered through this site has facilitated numerous studies in Recommender Systems.

My approach is:
1. Remove duplicate tags (remove capitalization and punctuations)
2. Identify similar tags with the same stem (stemming) and keep only the one with highest quality
3. Train word2vec model on IMDB movie reviews, and use the model to identify tags with similar syntactic meanings. 
Filter out low-quality ones and keep only the one with highest quality.
4. I generate a new table that keep track of only high quality tags, write a python script to update the tag data 
in Movielens' database.
