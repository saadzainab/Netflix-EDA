# Netflix Dataset — Exploratory Data Analysis

**FAST-NUCES | Data Science — Assignment 2**

## Project Overview

This project performs Exploratory Data Analysis (EDA) on the Netflix Movies and TV Shows dataset to understand content distribution, release trends, maturity ratings, genres, countries, and durations.

The analysis includes data quality assessment, cleaning, feature engineering, and statistical visualizations to identify meaningful patterns in Netflix's catalogue.

## Dataset Information

- **Dataset:** Netflix Movies and TV Shows
- **Original Records:** 8,807
- **Original Features:** 12
- **Cleaned Features:** 18
- **Data Format:** CSV

The dataset contains information about Netflix titles, including content type, release year, date added, director, cast, country, rating, duration, and genre.

## Tools and Libraries

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Jupyter Notebook / Google Colab

## Assignment Tasks

| Section | Description |
|---|---|
| A1 | Dataset Understanding |
| A2 | Data Quality Assessment |
| A3 | Data Cleaning and Feature Engineering |
| A4 | Univariate EDA |
| A5 | Bivariate EDA |
| A6 | Multivariate EDA |
| A7 | Netflix-Specific Analytical Questions |
| A8 | Key Insights and Assignment 3 Handoff |

## Data Cleaning

The following cleaning operations were performed:

- Removed unnecessary whitespace from text columns.
- Corrected three misplaced duration values in the rating column.
- Replaced missing categorical values with `"Unknown"`.
- Converted `date_added` into datetime format.
- Retained missing dates and valid unusual observations.
- Separated movie durations and TV-show season counts.
- Created six derived variables: `year_added`, `release_gap`, `movie_minutes`, `seasons`, `num_countries`, and `num_genres`.

**Note:** Empty values in `movie_minutes` for TV Shows and `seasons` for Movies are intentional because these measurements are not applicable to the opposite content type.

## Key Findings

1. Movies represent approximately **69.6%** of the catalogue, while TV Shows account for 30.4%.
2. TV Shows generally have more recent release years than Movies.
3. The United States, India, and the United Kingdom are among the most represented countries.
4. TV-MA and TV-14 are the most common maturity ratings.
5. The median movie duration is approximately **98 minutes**, while most TV Shows have one season.


## Conclusion

The analysis provides an overview of Netflix's catalogue through data cleaning, statistical summaries, and visualizations. The cleaned dataset and derived features establish a foundation for further analysis in Assignment 3.
