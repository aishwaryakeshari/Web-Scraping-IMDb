# Web-Scraping-IMDb
Link to the notebook: https://jovian.ai/aishwaryakeshari18/web-scraping-imdb-tv-shows

**Web Scraping** is process of collecting information from a website in an automated manner using code. This information is collected and then exported into a format that is more useful for the user. I will be using the libraries [Requests](https://docs.python-requests.org/en/master/index.html) and [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) in Python to scrape data from the website.

[IMDb](https://www.imdb.com/) is the world's most popular website that contains information about TV Shows, movies, video games, and streaming content online – including cast, production crew, plot summaries, trivia, ratings, fan and critical reviews and a lot more. It is designed to help fans explore the world of movies and shows and decide what to watch.

Here is the outline of the steps that I am planning to follow:
1. Import the required libraries and download the website using `requests`
2. Parse the HTML source code using `BeautifulSoup`
3. Extract the top 250 TV Shows rank, title, release year, IMDb ratings, genre, runtime, and plot summary from the website
4. Complie extracted information into Python dictionaries and `Pandas` DataFrame
5. Save the extracted information to a CSV file. 

By the end of the project I will create a CSV file in the following format:

```
Rank, Title, Release Year, IMDb Ratings, Genre, Runtime, Plot Summary
1, Planet Earth II, 2016, 9.5, Documentary, 4h 58min, Wildlife documentary series with David Attenborough, beginning with a look at the remote islands which offer sanctuary to some of the planet's rarest creatures, to the beauty of cities, which are home to humans, and animals..
2, Planet Earth, 2006, 9.4, Documentary, 8h 58min, Emmy Award-winning, 11 episodes, five years in the making, the most expensive nature documentary series ever commissioned by the BBC, and the first to be filmed in high definition.	
....
```
