# MyMo--A-Movie-Recommendation-System

### INTRODUCTION

In the world of growing digital media and digital platforms, it is difficult to search through all the available content to choose one, be it in the field of consumer products (shopping websites and applications), eBooks, videos, or movies. Also, with the advent of new platforms, there is a competition among the providers to increase the customer engagement on their platform.
A recommendation system eases the decision-making process for people by filtering or sorting out the content on the basis of their past behaviors. The better the recommendation system, better is the engagement on the platform. We all have seen this in our day to day lives, as we are more inclined towards websites and apps where we can easily find content personalized to our liking rather than browsing through multiple pages.

MyMo is movie recommendation system which can suggest a list of 10 movies to any user.
Recommendation systems can be content based or collaborative filtering based. MyMo is a hybrid system which combines the results from both content and collaborative filtering methods.

### DATA

The dataset used for developing MyMo is the MovieLens Dataset.
The dataset contains 25,000,095 ratings and 1,093,360 tag applications across 62,423 movies. This data was created by responses from 162,541 users between January 09, 1995, and November 21, 2019.

### METHODOLOGY

In content-based filtering, only the items that a particular user has watched in the past are used to determine the new recommendation. 
The genre of a movie gives information about content of the movie which is used by Mymo for filtering out similar movies.
First the genres are converted to a vector using Count Vectorizer. It converts the given genre text into its frequency representation.

![image](https://user-images.githubusercontent.com/95187849/210449506-1a43246d-83a3-4c64-b406-86a640286e98.png)

Cosine similarity between these vectors is used to identify similar movies. Cosine similarity between two vectors is defined by 

![image](https://user-images.githubusercontent.com/95187849/210449642-806df343-1910-4a9e-bf65-aa0fbde7a8bd.png)


The basic concept of Collaborative filtering is that two or more people who have similar interests in one area will be inclined towards similar items or products.  
We used movie rating as the feature for finding out collaborative recommendations. 
In this method, we first determine the users who have watched and liked the same movie as us and then from all the movies that those similar users have watched, we create a list of movies which are liked by most of those users. 
To create the front end of MyMo, we have used tkinter library in Python.
It provides interface to the Tcl GUI toolkit. MyMo takes the name of movie as input and returns a list of top 10 recommendations.



### RESULTS AND CONCLUSION
MyMo combines the results from both the approaches and creates a curated list of 10 movies. These  recommendations are a simple combination of content based and collaborative recommendations.
![image](https://user-images.githubusercontent.com/95187849/210449718-f8c0c3a3-eeb6-4c47-bcab-ec1c8eb05383.png)


In future, along with the similarity index, clustering and classification techniques can be used to improve MyMo.
This approach can also be extended to recommend videos, books, news etc.





