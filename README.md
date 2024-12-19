# IMDB-Movie-Data-Scraping-and-Enrichment
## Project Overview

This project involves scraping data from IMDB to analyze top-rated movies released between 2018 and 2020, sorted by user votes. The goal is to extract key movie details, clean and transform the data, and enrich an existing movie dataset with additional information from IMDB.

### The project involves the following key steps:

1. **Scraping IMDB Data**: The project uses web scraping techniques with the BeautifulSoup library in Python to extract details of top-rated movies from IMDB. Movies are filtered by their release dates (2018–2020) and sorted by the number of user votes. Data pulled for each movie includes:
    - Movie ID
    - Rank
    - Title
    - Runtime
    - Year of release
    - Rating (out of 10)
    - Number of votes

2. **Data Transformation and Cleaning**: After scraping the data, the project performs various data cleaning tasks such as:
    - Converting runtime to minutes
    - Handling missing values and correcting data inconsistencies (e.g., filling missing values with 'Not Rated' for the rating category)
    - Ensuring numeric consistency (e.g., converting votes to integer type)
    - Renaming and formatting columns for clarity

3. **Enrichment with Existing Dataset**: The project merges the scraped data with an existing movie dataset ("Movies.csv"). The resulting enriched dataset provides a comprehensive view of the top-rated movies, with the added IMDB data integrated into the dataset for further analysis.

4. **Exporting Data**: The final enriched dataset is exported to a CSV file for easy access and further analysis. The file includes movie details such as:
    - Movie ID
    - Rank
    - Title
    - Original Title
    - Description
    - Year
    - Number of Votes
    - Rating
    - Runtime (in minutes)
    - Rating Category
    - Genres

### Key Files in the Project

1. **IMDB_Movie_Scraping_Analysis.ipynb**: 
   - A Jupyter Notebook that contains the code for scraping the IMDB website, cleaning the data, and performing transformations. It also includes the logic for merging the scraped data with the existing dataset.

2. **TopVoted_IMDB_Movies_2018_2020.csv**:
   - A CSV file containing the scraped IMDB movie data, including movie details such as ID, rank, title, runtime, year, rating, and votes.

3. **Enriched_IMDB_Movie_Dataset.csv**:
   - The final enriched dataset combining the IMDB movie data with the original dataset. It includes a complete set of movie details, ready for analysis or further enrichment.

### Technologies Used

- **Python**: Used for web scraping, data cleaning, and data analysis.
- **BeautifulSoup**: For scraping HTML content from IMDB.
- **Pandas**: For data manipulation, cleaning, and transformation.
- **Jupyter Notebook**: For running and documenting the code in an interactive environment.
