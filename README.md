# IMDb Movie Data Acquisition and Cleaning Notebook

We live in a world full of digital footprints—every interaction we have online leaves behind clues about our behaviors, preferences, and decisions. But before these digital footprints become truly useful in understanding and predicting human behavior, there's quite a bit of work to do—like carefully collecting, cleaning, and structuring the data. 

This project walks through this process using data from the Internet Movie Database (IMDb). IIMDb is the largest database on films and filmmakers, containing records on who worked on which movie from 1900 to today. Audiences frequently use IMDb to find information about movies and TV shows, while industry professionals also rely on it for strategic decisions about hiring talent, investing in film projects, and understanding market dynamics.

In this notebook, I developed a pipeline to access and transform IMDb data into structured, clean datasets. Specifically, this project:
- Acquires data directly from IMDb's servers, which provides the most up-to-date information and eliminate the need for manual downloads and storage in local directories.
- Integrates multiple related IMDb datasets (movie information, ratings, filmmaker information) to create a comprehensive dataset.
- Preprocesses and cleans data, handling challenges such as missing values, duplicates, inconsistent formats, and data type mismatches.
- Provides initial insights into the industry through exploratory data analysis, uncovering trends in movie characteristics, team composition, and audience ratings. 


**Data Sources:**  
- IMDb Title Basics: Contains basic movie information such as movie IDs (`tconst`), title types, release years, genres, and runtime.
- IMDb Title Ratings: Provides movie ratings and the number of votes.
- IMDb Title Principals: Lists the people involved in the making of movies, including their IDs (`nconst`), professions, and the movies they have worked on.

**Key Skills:** Automated Data Acquisition, Data Cleaning & Transformation, Data Integration, Exploratory Data Analysis, Data Visualization

**Tools:** Python, Pandas, Matplotlib, Seaborn, Ast, Math, Unidecode, Scipy, Re

**Results:**
- Movie Dataset: Contains 300,000+ movies released between 2000 and 2024, with detailed metadata, including movie IDs, titles, genres, release years, ratings, and popularity metrics.
- Filmmaker Dataset: Contains 600,000+ filmmakers working in creative roles, with detailed metadata, including filmmaker IDs, names, professions, and the movies they have worked on.

These datasets serve as the foundation for my PhD dissertation, where I conducted dynamic network analysis and predictive modeling to understanding factors driving the success of films and filmmakers.

## Visualizing Trends in the Movie Industry between 2000 and 2024

![Movie Production Trends](image/num_movies_2000_2024.png)

![Genre Popularity Trends](image/genre_popularity_2000_2024.png)

![Share of Creative Roles](image/creative_roles_percentage_2000_2024.png)


## How to Run the Code

1. **Clone the Repository:**  
   ```bash
   git clone https://github.com/nhunguyen0901/imdb-data-acquisition-cleaning.git
   cd imdb-data-acquisition-cleaning

2. **Install Dependencies:**
Ensure Python is installed, and then set up the required libraries using:
    ```bash
    pip install -r requirements.txt

3. **Run the Notebook:**
Open the Jupyter Notebook file (`IMDb_Data_Acquisition_Cleaning.ipynb`) using Jupyter Notebook or JupyterLab. Follow the cells sequentially to reproduce the results.


