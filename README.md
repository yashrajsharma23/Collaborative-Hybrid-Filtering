# Collaborative-Hybrid-Filtering
Using of matrix factorization collaborative filtering and hybrid neural collaborative filtering

## Dataset Description:
The dataset is from the MovieLens dataset collected by the GroupLens Research Project at the University of Minnesota. 
This data set consists of:
	* 100,000 ratings (1-5) from 943 users on 1682 movies. 
	* Each user has rated at least 20 movies.
Here are brief descriptions of the data:

### ratings.txt    
-- The full 'u' data set, 100000 ratings by 943 users on 1682 items. Each user has rated at least 20 movies.  Users and items are numbered consecutively from 1.  The data is randomly ordered. This is a tab-separated list of 
	         user id | item id | rating | timestamp. 
The timestamps are Unix seconds since 1/1/1970 UTC

### movies.txt    
-- Information about the items (movies); this is a tab-separated list of
              movie id | movie title | release date | video release date |
              IMDb URL | unknown | Action | Adventure | Animation |
              Children's | Comedy | Crime | Documentary | Drama | Fantasy |
              Film-Noir | Horror | Musical | Mystery | Romance | Sci-Fi |
              Thriller | War | Western |
The last 19 fields are the genres.  A 1 indicates the movie is of that genre, a 0 indicates it is not; movies can be in several genres at once. The movie ids are the ones used in the u.data data set.

### genre.txt    
-- A list of the genres

## Architectures
### 1. Matrix Factorization
Architecture

![Matrix-Factorization](https://user-images.githubusercontent.com/39268487/129469769-360f882d-4117-491d-b974-3e940d005134.png)


Values & Loss of ratings prediction

![matrix-factorization (2)](https://user-images.githubusercontent.com/39268487/129469795-0241049f-6c0a-4715-b696-5f7b293fe0af.PNG)


### 2. Hybrid Neural Collaborative Filtering
Architecture

![Hybrid-Diagram-2](https://user-images.githubusercontent.com/39268487/129469780-fb23c2f1-2494-4893-a325-be6cb7c556a6.png)

Embedding Layer

![embedding](https://user-images.githubusercontent.com/39268487/129469844-edde4d90-7c6b-45fd-857c-2a7c11e2b8d5.png)


Neural Embedding Layers

![hybrid](https://user-images.githubusercontent.com/39268487/129469804-6eaaa84f-b79b-4fc9-872b-340470419a67.PNG)

### Loss of Matrix Factorization & Hybrid

![both-recommender](https://user-images.githubusercontent.com/39268487/129469835-4846457b-249c-4adf-8ee7-33f04769a240.PNG)

