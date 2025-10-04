# Netflix Dataset Analysis

## Project Description

This project aims to analyze Netflix's content library to understand the trends in content distribution, including the mix of Movies and TV Shows, popular genres, and contributions from different countries. The insights gained from this analysis can help Netflix in strategic content acquisition and production decisions.

## File Structure and Dependencies

*   `Netflix Dataset.csv`: The dataset containing information about Netflix titles.
*   `netflix_cleaned.csv`: The cleaned dataset generated after data preprocessing.
*   This notebook: Contains the code for data loading, cleaning, EDA, and visualization.

**Dependencies:**

*   pandas
*   matplotlib
*   seaborn

## Data Source

The dataset used in this project is the "Netflix Movies and TV Shows" dataset, which is publicly available and contains a comprehensive list of titles available on Netflix, along with associated metadata such as director, cast, country, release year, rating, duration, and genre.

## Data Cleaning and Preparation

The following data cleaning steps were performed:

*   Missing 'Country' entries were filled with 'Unknown'.
*   The 'Release_Date' column was converted to datetime objects.
*   The 'Release_Year' was extracted from the 'Release_Date' column.
*   Missing 'Rating' values were replaced with 'Not Rated'.
*   The 'Country' column was processed to extract the 'Main_Country' for each title (taking the first country listed).

## Exploratory Data Analysis (EDA)

The EDA section explores the cleaned dataset through various visualizations to understand the content landscape on Netflix. Key analyses include:

*   **Distribution of Movies vs TV Shows:** Visualizing the proportion of movies and TV shows in the dataset.
*   **Content Releases by Year:** Analyzing the trend of content releases over the years using a bar plot.
*   **Top Content-Producing Countries:** Identifying the countries with the highest number of titles on Netflix using a bar plot.
*   **Top Genres/Types:** Exploring the most frequent genres and types of content available on the platform through a bar plot.
*   **Year-wise Trend: Movies vs TV Shows:** Visualizing the yearly trend of movie and TV show releases using a line plot.

## Code Structure

The notebook is structured into the following sections:

1.  **Problem Statement:** Defines the project's objective.
2.  **Import Libraries:** Imports necessary Python libraries.
3.  **Load Dataset:** Loads the Netflix dataset into a pandas DataFrame.
4.  **Data Cleaning:** Contains code for handling missing values and data type conversions.
5.  **EDA:** Includes code for generating visualizations to explore the data.
6.  **EDA Findings:** Summarizes the key observations from the EDA.
7.  **Save Cleaned Data:** Saves the processed data to a new CSV file.

## Key Findings and Recommendations

*   Netflix has a significantly higher number of movies compared to TV shows.
*   The platform has experienced substantial growth in content releases over the years, particularly since 2016.
*   The United States is the primary content contributor, followed by India and the United Kingdom.
*   International Movies, Dramas, and Comedies are the most dominant genres.

**Recommendations:**

*   Continue to invest in International Movies, Dramas, and Comedies, as they are popular genres.
*   Explore opportunities to expand content production or acquisition from countries with growing contributions.
*   Analyze the 'Unknown' country data to identify potential emerging markets or content sources.

## How to Run the Notebook

1.  Ensure you have the required libraries (pandas, matplotlib, seaborn) installed.
2.  Download the "Netflix Movies and TV Shows" dataset (`Netflix Dataset.csv`) and place it in the same directory as the notebook.
3.  Run the cells sequentially in the notebook.
4.  The cleaned data will be saved as `netflix_cleaned.csv`.
