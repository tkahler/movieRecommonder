# movieRecommender
A movie recommender. Enter a movie at tkrecommender.me and list of movies similar to the movie entered will be returned.

Uses simpleHTTPServer CGI request handler (webServer.py) to run the python script that processes recommendations, server-side.

User can input a movie into a form and list a movies similar to the entered movie will be returned.

Currently any movie can be entered and found through the omdb (open movies database) and will be compared to a database of IMDB's top 250 movies. 

Recommendation Algorithm: 
Using the genre, actors, directors and keywords from the plot, a bag of words vector is created, then the a cosine similarity matrix is made between the movie entered and the movies within the database. The top ranked movies are selected and displayed.

