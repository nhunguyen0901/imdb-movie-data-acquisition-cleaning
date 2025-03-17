# IMDb Movie Data Acquisition and Cleaning Notebook

Large digital trace datasets provide a wealth of information about human behavior and interactions, but they often require extensive cleaning and preprocessing before they can be used for analysis. This project focuses on acquiring and cleaning data from the Internet Movie Database (IMDb) to create a structured dataset for further analysis. The Internet Movie Database (IMDb) provides detailed records on movies and the people who work on them—data that spans an entire multi-billion-dollar industry from 1900 to the present. It is often used by audience to find information about movies, TV shows, and video games, and by professionals to research the industry and make decisions about hiring, investing, and producing. 

The resulting dataset captures a wide range of 300,000+ movies spanning over two decades (2000-2024), with detailed information on movie titles, genres, release years, ratings, and more. It serves as the foundation for my PhD dissertation analyses, including dynamic network analysis and predictive modeling to understanding factors that influence success of films and filmmakers.

## Project Overview

**Data Sources:**  
- **IMDb Title Basics:**  
  Contains basic movie information such as movie IDs (`tconst`), title types, release years, genres, and runtime.
- **IMDb Title Ratings:**  
  Provides movie ratings and the number of votes, which are merged with the title basics data.

**Techniques Used:**  
- **Data Acquisition:** Utilizing Python's `requests` and `zipfile` libraries to download and extract data from IMDb's server, which provide the most up-to-date information and eliminate the need for manual downloads and storage in local directories.
- **Data Integration:** Merging datasets from different sources to enrich the data for comprehensive analysis.
- **Data Cleaning and Transformation:** Converting data types, identifying and addressing duplicates and missing values, filtering rows based on specific criteria, and standardizing genre information.
- **Exploratory Analysis:**  
  Generating summary statistics and visualizations (histograms, bar charts) using `pandas`, `matplotlib`, and `seaborn` to understand the distribution of key variables and trends over time.


## How to Run the Code

1. **Clone the Repository:**  
   ```bash
   git clone https://github.com/nhunguyen0901/imdb-data-acquisition-cleaning.git
   cd imdb-data-acquisition-cleaning

2. Install Dependencies:
Make sure you have Python installed (preferably Python 3.7+). Then, install the required libraries using:

