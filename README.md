# Netflix-Recommendation-System
Netflix is an organization that maintains a vast range of TV shows and videos, distributing them online which are accessible anytime. To keep the users glued to the platform without losing interest, providing suggestions to the users becomes essential.  Netflix Recommendation System helps to increase customer engagement, user satisfaction, and to better understand what the user wants. This system recommends movies most popular to the users based on most-watched movies &amp; having high ratings.

# movie_titles.txt
This file contains MovieID, YearOfRelease and Title of the movie. Movie ids are not the actual Netflix movie ids or IMDB movie ids. YearOfRelease ranges for 1890 to 2005 and corresponds to release of DVD and not the actual theatrical release. Title is Netflix movie title in English.

# Idea behind the recommendation system
1. We start by importing all the libraries and the dataset.
2. Then, we visualise the ratings by customers on Netflix based on movie count, customer count and ratings count.
3. We can see that the score continues to be relatively positive (>3). This may be because dissatisfied consumers choose to just quit instead of trying to rate. We should have    this in mind because low-rating movies usually suggest that they are very poor.
4. As movie ID column is a mess, we can simplify this by first making a NumPy array of the right length, then inserting the whole array as a column in the main data frame.
5. To reduce the volume of the data, keeping data quality in mind we perform two tasks. Firstly, if the ratings of the movies are less than a benchmark, delete the movie as it    might be unpopular. Secondly, remove the customers who give less notice as he might be less interactive than the others.
6. Then, in the Netflix recommendation algorithm, we extract the movies that correspond to the movie for which we are giving recommendations. Then, we find the PearsonR score      of those movies and recommend the movies having the top 10 values for PearsonR score.

# Usage License – Netflix
Netflix can not guarantee the correctness of the data, its suitability for any particular purpose, or the validity of results based on the use of the data set.
The data set may be used for any research purposes under the following conditions:
* The user may not state or imply any endorsement from Netflix.
* The user must acknowledge the use of the data set in publications resulting from the use of the data set and must send us an electronic or paper copy of those publications.
* The user may not redistribute the data without separate permission.
* The user may not use this information for any commercial or revenue-bearing purposes without first obtaining permission from Netflix.
If you have any further questions or comments, please contact the Prize administrator <prizemaster@netflix.com>
