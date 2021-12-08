# cs50finalproject
Movie Magic - CS50 Final Project
# Movie Magic - CS50 Final Project by Haley Mosdell
This project was designed for the movie lovers out there. When the world shut down in March 2020, I found myself with a lot more free time than I had ever had. I no longer had to commute to the office for 30+ minutes each day, so I decided to start watching movies I had been intending to watch for years with that free time. Oscar movies, classics, you name it! I hadn't yet seen Forrest Gump, if you can believe it! I started to write down a list of movies and began checking them off as I watched them, manually writing down a rating for each. Later, I lost the notebook with this list in the shuffle of a move and at 300+ handwritten titles, I wished I had stored the information elsewhere as it was gone for good!

This was the inspiration for my final project, Movie Magic! Movie Magic is a Flask App written with Python, HTML, CSS and JavaScript with a database in SQLAlchemy. Movie Magic uses TMDB's API to pull popular movies from TMDB as well as dynamically search for titles. Through these different search/browse views, you can add movies to your "Watchlist" to generate a list of titles that you want to watch, or add them to your "Favorites"!

## Getting Started
Make sure you have the latest version of Python installed on your computer.

In your terminal, run the following commands in order to access all the libraries used.

```Python
pip install Flask
```
```Python
pip install SQLAlchemy
```
```Python
pip install Flask-Login
```
```Python
pip install better_profanity
```
And that's all the requirements to run this Flask app! You can start using the app by executing

```Python
flask run
```
in VSCode

### Login
The first view you will see when you open the app is the login page. Follow the link to the "Register" page or access the "Register" page in the navigation bar.

### Register
Register with a valid email address and set a username and password.

### Home
On the homepage you will see a summary of all of your recent activities on the app. When you first login, there will be nothing here. Follow any of the links to either browse titles or make posts!

Once you start adding movies, the leftmost column will display your 3 most recently added movies in descending order. The middle column will show your 3 most recently favorited movies in descending order. The rightmost column is your 3 most recent posts to "Community"!

### Movie Cards
On each movie card, you will find the poster image, title, release date and hover to see the overview! You may find from one page to another, the buttons look a little different. This is by design to allow you to toggle movies between "Favorites" and "Watchlist" and dynamically delete cards.

Note: for some less well known titles accessed via "Search" you may find some information missing.

### Watchlist
Your "Watchlist" is meant for movies you plan to watch! You can add anything to your "Watchlist" by browsing titles in the "Popular" page or via search simply by clicking "Watchlist" on any given movie card. 

From this view, you can delete movies if you change your mind, or you can add them to "Favorites" once you've watched them!

### Favorites
Your "Favorites" are movies you've already seen. You can browse titles and keep track of movies you watched and enjoyed. You can also add movies to "Favorites" from "Watchlist"

### Popular
"Popular" pulls the current most popular titles from The Movie Database's API! This will update and render live on the page, so this page will look different from day to day!

From this view, you have three sort options to organize the current post popular titles: in order of most popular/relevant, in order of rating, or in alphabetical order.

For more information on TMDB's API:
[Click here](https://developers.themoviedb.org/3/getting-started/introduction)

### For Me/Recommendations
"For Me" takes an average rating from all of the movies you've added to search, as well as your top 3 most occurring genres from favorites to perform a compound search on TMDB's available titles, which is automatically sorted by relevance and popularity.

As you add more movies to your "Favorites" Movie Magic will better understand your genre preferences and make appropriate recommendations. 

### Community
"Community" is a simple blog that allows you to post your thoughts on any of the movies you've watched or interact with other users. Community includes a profanity filter from better-profanity to filter against posts with profanity.

Via "Community", you can access a given user's profile to browse their most recent activity. This page will look exactly like your homepage.

### Search
"Search" runs a title search on TMDB's database and sorts all titles by most relevant according to your search. Add any cards that appear to "Watchlist" or "Favorites"!

### Future Design Improvements
#### More JavaScript! 
Send error messages to the client side when a user tries to add a duplicate title to one of their lists

Keep buttons checked if a user has the movie already in their "Watchlist" or "Favorites" (Currently, this is a bit difficult to do as "Search" and "Popular" render results directly from TMDB API)

Allow users to rate their favorites with a star rating and fill in their rating our of 5 stars

#### A more robust community of users
More functionality for posts: adding, deleting, liking, comments

Ability to see other user's lists

"Add" or "Follow" other users and have a feed of other user's activities

Recommendations for users to follow based on common interests

#### Smart recommendation system
NLP models to access content from your favorited movies (by rating) to make better recommendations of movies to watch

###### Final Notes
I had a lot of fun designing and building this project and I hope you have fun playing around with it! I wish I had more time to make the site more robust, but I plan to continue with this template and add to it beyond CS50. Thank you! This was CS50 :)
