# Movie Recommendation System

This project is a Python script for generating movie recommendations based on a list of one or more movie titles. The recommendation process involves fetching related movie titles and sorting them based on their Rotten Tomatoes ratings. It leverages external APIs for fetching movie data and related titles.

> ## Note on TasteDive API
> 
> As of the writing of this README, the TasteDive API, which was originally used to fetch related movie titles, is no longer operational. As a result, the `get_movies_from_tastedive` function will not work as intended. Users looking to utilize this script will need to find an alternative API or method for generating related movie titles.

## Project Structure

- `movie_recommendation.py`: The main Python script that includes functions for fetching related movie titles, extracting movie data from the OMDb API, and sorting movies based on their ratings.

### Prerequisites

- Python 3.x
- `requests` library (can be installed via pip with `pip install requests`)
- An API key for the OMDb API

### How to Run

1. Install Python from [python.org](https://python.org) and the `requests` library by running `pip install requests` in your terminal or command prompt.
2. Get an OMDb API key from [OMDb API](http://www.omdbapi.com/apikey.aspx).
3. Download the script files to your computer.
4. Open `movie_recommendation.py` and insert your OMDb API key where indicated.
5. In your terminal or command prompt, navigate to the script's directory.
6. Execute the script with `python movie_recommendation.py`.
7. Input your movie titles as prompted by the script.

## Functions Overview

- `get_movies_from_tastedive(name)`: Fetches related movie titles from TasteDive (note: this function is currently non-operational).
- `extract_movie_titles(json_data)`: Extracts movie titles from the JSON data returned by an API.
- `get_related_titles(titles)`: Finds related titles for a list of movies.
- `get_movie_data(title)`: Fetches movie data from the OMDb API.
- `get_movie_rating(json_data)`: Extracts the Rotten Tomatoes rating from the movie data.
- `get_sorted_recommendations(movie_list)`: Generates a list of recommended movies sorted by Rotten Tomatoes ratings and alphabetically.

## License

This project is open source and available under the [MIT License](LICENSE.md).

## Acknowledgments

- Thanks to the creators of the APIs that made this project possible.
- Special acknowledgment to the developers and community around the Python `requests` library for their invaluable tool.

