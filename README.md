# IMDB Top 1000 Movie Rankings Explored

## Overview

This EDA focuses on a dataset of IMDB's Top 1000 Movie rankings.

The analyis first takes a brief look at the entire dataset of 1000 movie entries. Then, it shifts its focus onto the top 1% performing movies.

## Research Questions
### General Correlations
- Are there any correlations present between the various informations regarding a popular box office movie?
- If so, what do these correlations look like, i.e. how strong are these correlations? Which factors influence others?

### Specific Viewership Relations
- Are there differences between how the general population rate movies and how critics score movies?
- Is the gross of a movie affected by either kinds of reception?

## Data and Methodology
### Original Source

The dataset used is the [IMDB Movies Dataset hosted on Kaggle](https://www.kaggle.com/datasets/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows).

It contains information from the top 1000 rated movies from IMDB in CSV format.

### Starting Information

For each movie, the original dataset's columns contained the following information:

- A hyperlink to a **poster** of the movie
- **Title** of the movie
- **Year** the movie was released
- Country-specific **certificates**
- **Runtime**, length of the movie, in hours and minutes
- The movie's **genre(s)** (1)
- **IMDB rating**, an average rating out of 10 that is open to the general audience via the IMDB website
- **Overview**, the synopsis of the movie's
- **Metacritic score**, an average score system out of 100 that is available only to professional movie critics
- **Director** of the movie
- **Starring** actors and actresses (4)
- Number of **IMDB rating votes**
- **Gross** of the movie when it was released

### Trimmed Down

To make a comparisons possible, data columns were removed, converted into usable types, and then consolidated:

- **Title**, e.g. "The Dark Knight"
- **Year**, "2008" `(converted from string to integer)`
- **Runtime**, "152" `(now in minutes)`
- **Genre**, "Action, Crime, Drama" `(split per genre)`
- **IMDB rating** "9.00"
- **Metacritic score**, "84.00"
- **Director**, "Christopher Nolan"
- **Stars**, "Christian Bale, Heath Ledger, ..." `(split per star)`
- **IMDB votes**, "2303232"
- **Gross adjusted**, "642923201.61" `(adjusted for inflation via average CPI formula)`

The resulting dataset contained a mix of numeric data columns, and non-numeric string columns.

This allowed making generalized statements about the dataset based on quantitative value-based comparisons, as well as specific statements regarding relations between the qualitative categories.


## Contextual Visualization
### Correlational Heatmap
To glean any big-picture information, the correlational coefficient was obtained for the numeric data columns:

![Table](img/corr_table.png)


The correlational heatmap generated based on results:

![Heatmap](img/corr_heatmap.png)

Bar graph of the strength of correlational coefficients:

![Bar](img/corr_bar.png)

## Specific Visualizations
* **Purpose:**
* **Details:**
* **Example:**

## Recommendations
* **Purpose:**
* **Details:**

## Future Areas of Research
* **Purpose:**
* **Details:**

## End Briefing / Final Slide
* **Purpose:**
* **Details:**