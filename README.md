
# Webscraping Popular Movies and TV Shows from TMDB

### Using Python, Requests and Beautifulsoup4

## Introduction:

The Movies Database or [TMDB]("https://www.themoviedb.org/") is a popular website hosting information about the millions of the movies, TV Shows and People from the Entertainment Industry. We will scrape some of this data to build our WebScraping Project.

This project is a part of DataScience and MachineLearning Bootcamp Course hosted on [Jovian]("https://jovian.ai/learn/zero-to-data-analyst-bootcamp").

[Web Scraping]("https://en.wikipedia.org/wiki/Web_scraping") any website involves fetching a page and extracting data from it. Fetching is the downloading of a page (which a browser does when a user views a page).

There are many tools/libraries like WebScrapper, Octoparse, Web Chrome Extensions which can scrape the information. 

Here in this project we will Web Scrape TMDB web site using Python libraries like [Requests]("https://pypi.org/project/requests/") and [BeautifulSoup4]("https://www.crummy.com/software/BeautifulSoup/bs4/doc/"). We will build many functions to extract handful of features to build our dataset. We will write the dataset information in the CSV format.

We will scrape TMDB Website to extract data for the Popular Movies and TV Shows from TMDB. 

## Outline of the Project:

1. Download TMDB Web Page.

2. Parse the HTML code of webpage.

3. Extract the data from the parsed HTML page in dictionary.

4. Create a list of data in dictionaries.

5. Write data to CSV using Pandas DataFrame.


## Detailed Plan of the Project:

1. Download the TMDB [Popular Movies Webpage](https://www.themoviedb.org/movie) or [Popular TV Shows WebPage](https://www.themoviedb.org/tv) using requests library.

2. Parse the webpage using BeautifulSoup4. WebPage contains information about the 20 TV Shows.

3. Extract following data for each of 20 movies or shows depending on your choice of webpage given above.

-- Title
-- Release Date
-- URL


4. With the requests library download the TV Show webpage using the URL from above step.

5. Parse the Popular Movie or TV Show WebPage using Beautiful Soup Library.

6. Write functions to extract information from the Parsed HTML Page. The details extracted for each TV Show include:

a. Genres
b. Runtime
c. User_like_percentage
d. Original Language
e. Network URL
f. Writers
g. Writers URL
h. Cast Members

i. current season
j. number of episodes in current season

**OR** 

If you have chosen Movies Webpage, then most of functions to extract information for individual movie remains same (marked a-h above) except for last two functions which will extract:

k `budget`
l 'revenue'

7. Write this extracted data including the one extracted at Step 3 into a python Dictionary.

8. Repeat the **Step 4-7** for all of the 20 Movies/Shows displayed on WebPage.

9. Create a list of dictionaries with information about 20 Popular Movie / TV Shows.

10. Repeat the steps from 1-9 to load more pages by selecting page next WebPage by specifying page number.

11. Write the extracted information into a CSV file in the format like:
release_date, title, url, genres, run_duration, user_like_percentage, original_language, budget*, revenue*, main_characters, cast.

In case of TV Shows instead of budget and revenue, we will extract current_season and num_episodes_current_season.

[Code and Notebook Link](https://jovian.com/shubhdak/webscraping-tmdb)
