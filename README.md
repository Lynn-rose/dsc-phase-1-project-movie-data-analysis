# MICROSOFT MOVIE STUDIO EDA

## Project Overview

For this project, we will use exploratory data analysis to generate insights for microsoft organisation to look after as they look forward to venture in the movie industry.

### Business Problem

Microsoft sees all the big companies creating original video content and they want to get in on the fun. Microsoft decides to create a new movie studio, but doesn't know anything about creating movies. Therefore we are to explore what types of films are currently doing the best at the box office. We then  translate those findings into actionable insights that the head of Microsoft's new movie studio can use to help decide what type of films to create.
In order to answer this, we try the following objectives.

### Objectives:

1. Which genres have the highest rating?
2. What is the coorelation between production budget, domestic gross and worldwide gross?
3. What is the popularity of a movie depending on the month it was released?

So, in addition to completing the basic data cleaning tasks and the aggregation and reshaping tasks needed to answer the question above, we'll also need to give feedback or conclusion on what microsoft needs to venture in.

## Data Understanding
Note that this data may not reflect the most up-to-date box office information.

The data is contained in two separate CSV files and a sqlite database :
1. `tmdb.movies.csv` : each record represents a movie with attributes of the movie (e.g language,release date). This data was collected from [TheMovieDB](https://www.themoviedb.org/)
2. `tn.movie_budgets.csv` : each record represents a movie with the production budget, domestic gross and worldwide gross. This data was collected from [The Numbers](https://www.the-numbers.com/)
3. `im.db` :  SQLite database where `movie_basics` and `movie_ratings` tables are the most relevant. This data was collected from [IMDB](https://www.imdb.com/)

Because it was collected from various locations, the different files have different formats. Some are compressed CSV (comma-separated values)  files that can be opened using spreadsheet software or `pd.read_csv`, while the data from IMDB is located in a SQLite database.

![movie data erd](https://raw.githubusercontent.com/learn-co-curriculum/dsc-phase-1-project-v2-4/master/movie_data_erd.jpeg)

Note that the above diagram shows ONLY the IMDB data. You will need to look carefully at the features to figure out how the IMDB data relates to the other provided data files.

## Data Analysis
Perform Data Cleaning and Agreggation Required to Answer the Objectives.

1. Which genres have the highest rating?
2. What is the coorelation between production budget, domestic gross and worldwide gross?
3. What is the popularity of a movie depending on the month it was released?

## Findings

1. We get to see that the genre combination of Comedy, Documentary, Fantasy has the highest rating of 9.4 while the genre combination of comedy, musical, sport has the lowest rating of 1.4. ![Genre Rating Relationship](https://github.com/Lynn-rose/dsc-phase-1-project-movie-data-analysis/blob/master/images/genres.png)
2. We get to see that production budget and domestic gross have a positive correlation of 0.6856818396752724.![Genre Rating Relationship](https://github.com/Lynn-rose/dsc-phase-1-project-movie-data-analysis/blob/master/images/production%20budget%20vs%20domestic%20gross.png)
3. we as well see this in both production budget and worldwide gross having a correlation of 0.7483059765694747.![Genre Rating Relationship](https://github.com/Lynn-rose/dsc-phase-1-project-movie-data-analysis/blob/master/images/production%20budget%20vs%20worldwide%20gross.png)
4. We get to see that a movie released in December has more popularity than a movie released in January or April.![Genre Rating Relationship](https://github.com/Lynn-rose/dsc-phase-1-project-movie-data-analysis/blob/master/images/popularity%20based%20on%20month.png)

# Conclusion
 
## Recomendations

Based on the findings of each objective, we find the following recomendations worthwhile for microsoft organisation to look after as they look forward to venture in the movie industry.
1. venture into the genre combination of Comedy, Documentary, Fantasy has the highest rating than the rest meaning the audience highly recommend the genre combination. this is true as the analysis looked at the average rating of different movies having this combination and this was found to be the feedback.
2. We have a positive coorelation between production budget and domestic gross as well as a positive correlation between production budget and worldwide gross. This means that the higher the production budget the higher the domestic gross and the worldwide gross. Therefore,having a higher production budget will be more profitable to the organisation
3. The popularity of a movie is quite dependent on the time the movie is released. Going by this we see that when a movie is released in December the movie will be more popular than releasing the movie in the rest of the months.

 ## For More Information  
Please review my full analysis in my [Jupyter Notebook](https://github.com/Lynn-rose/dsc-phase-1-project-movie-data-analysis/blob/master/student.ipynb) or my [Presentation](https://github.com/Lynn-rose/dsc-phase-1-project-movie-data-analysis/blob/master/presantation.pdf)

For any additional questions, please contact Lynn Rose Achieng, lynn90952@gmail.com

