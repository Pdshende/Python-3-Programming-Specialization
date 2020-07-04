 
# course_3_project

--------------------------------

# Due: 2018-11-25 01:37:00

-------------------------

# Questions

------------------------
`

This project will take you through the process of mashing up data from two different APIs to make movie recommendations. The TasteDive API lets you provide a movie (or bands, TV shows, etc.) as a query input, and returns a set of related items. The OMDB API lets you provide a movie title as a query input and get back data about the movie, including scores from various review sites (Rotten Tomatoes, IMDB, etc.).

You will put those two together. You will use TasteDive to get related movies for a whole list of titles. You’ll combine the resulting lists of related movies, and sort them according to their Rotten Tomatoes scores (which will require making API calls to the OMDB API.)

To avoid problems with rate limits and site accessibility, we have provided a cache file with results for all the queries you need to make to both OMDB and TasteDive. Just use requests_with_caching.get() rather than requests.get(). If you’re having trouble, you may not be formatting your queries properly, or you may not be asking for data that exists in our cache. We will try to provide as much information as we can to help guide you to form queries for which data exists in the cache.

Your first task will be to fetch data from TasteDive. The documentation for the API is at https://tastedive.com/read/api.

Define a function, called get_movies_from_tastedive. It should take one input parameter, a string that is the name of a movie or music artist. The function should return the 5 TasteDive results that are associated with that string; be sure to only get movies, not other kinds of media. It will be a python dictionary with just one key, ‘Similar’.

Try invoking your function with the input “Black Panther”.

HINT: Be sure to include only q, type, and limit as parameters in order to extract data from the cache. If any other parameters are included, then the function will not be able to recognize the data that you’re attempting to pull from the cache. Remember, you will not need an api key in order to complete the project, because all data will be found in the cache.

The cache includes data for the following queries:


![pic1](https://github.com/Pdshende/Python-3-Programming-Specialization/blob/master/picture/Screenshot%20from%202020-07-04%2021-28-56.png)


```
# some invocations that we use in the automated tests; uncomment these if you are getting errors and want better error messages

# get_movies_from_tastedive("Bridesmaids")

# get_movies_from_tastedive("Black Panther")

import requests_with_caching

import json


def get_movies_from_tastedive(title):

    endpoint = 'https://tastedive.com/api/similar'

    param = {}

    param['q'] = title

    param['limit'] = 5

    param['type'] = 'movies'

    this_page_cache = requests_with_caching.get(endpoint, params=param)

    return json.loads(this_page_cache.text)
```
------------------------------------------------------------

Please copy the completed function from above into this active code window. Next, you will need to write a function that extracts just the list of movie titles from a dictionary returned by get_movies_from_tastedive. Call it extract_movie_titles.

```
# some invocations that we use in the automated tests; uncomment these if you are getting errors and want better error messages

# extract_movie_titles(get_movies_from_tastedive("Tony Bennett"))

# extract_movie_titles(get_movies_from_tastedive("Black Panther"))

import requests_with_caching

import json

def get_movies_from_tastedive(title):

    endpoint = 'https://tastedive.com/api/similar'

    param = {}

    param['q'] = title

    param['limit'] = 5

    param['type'] = 'movies'

    this_page_cache = requests_with_caching.get(endpoint, params=param)

    return json.loads(this_page_cache.text)

def extract_movie_titles(dic):

    list = []

    for i in dic['Similar']['Results']:

        list.append(i['Name'])

    return(list)
```

----------------------------------------

Please copy the completed functions from the two code windows above into this active code window. Next, you’ll write a function, called get_related_titles. It takes a list of movie titles as input. It gets five related movies for each from TasteDive, extracts the titles for all of them, and combines them all into a single list. Don’t include the same movie twice.


# some invocations that we use in the automated tests; uncomment these if you are getting errors and want better error messages

# get_related_titles(["Black Panther", "Captain Marvel"])

# get_related_titles([])

import requests_with_caching

import json


def get_movies_from_tastedive(title):

    endpoint = 'https://tastedive.com/api/similar'

    param = {}

    param['q'] = title

    param['limit'] = 5

    param['type'] = 'movies'

    this_page_cache = requests_with_caching.get(endpoint, params=param)

    return json.loads(this_page_cache.text)


def extract_movie_titles(dic):

    list = []

    for i in dic['Similar']['Results']:

        list.append(i['Name'])

    return(list)


def get_related_titles(titles_list):
    list = []
    for i in titles_list:
        new_list = extract_movie_titles(get_movies_from_tastedive(i))
        for i in new_list:
            if i not in list:
                list.append(i)
    print(list)
    return list
 ```
----------------------------------

