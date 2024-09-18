## Favorite Movies: Breakout Activity 1

To be completed on 2024-09-19 (Class 08).

## The Six Variables We're Focusing On Today

We will use the `movies_2024-09-17` data in the **Favorite Movies** directory on our Shared Drive, which describes 228 films mentioned as "favorites" by students in 431 for 2020-2024. 

There are six variables (`year`, `length`, `imdb_categories`, `imdb_ratings`, `imdb_stars` and `mpa`) that we will focus on today...

Variable | Sample Value | Explanation
:--------: | :------------: | ------------------------------------------------------------------------
`mov_id` | M-010 | code (1-228): arranges in alphabetical order by title, ignoring starting "The" or "A"
`movie` | Avengers: Infinity War | film title according to IMDB
**`year`** | 2018 | year film was released
**`length`** | 149 | length of film (in minutes)
**`imdb_categories`** | Space Sci-Fi, Superhero, Action, Adventure, Sci-Fi | Film Categories specified by IMDB (up to 10)
**`imdb_ratings`** | 1,200,000 | Number of Star Ratings (IMDB)
**`imdb_stars`** | 8.4 | Weighted Average Rating (IMDB)
**`mpa`** | PG-13 | Rating by the Motion Picture Association

The **Variable Descriptions** tab in the Google Sheet has additional information on all of these variables.

## Your Task(s) for Today

You'll have between 15 and 20 minutes to accomplish the following tasks.

1. Form a group of 4-6 people, at least one of whom you don't know yet. Come up with a group name that each of you will still remember in a week.
2. One person in your group will report the results of your work using the Google Form found at <https://bit.ly/431-2024-movies-1>. 
3. As a group, you will identify **two** exploratory questions about films in this sample that could be addressed using the six key variables (`year`, `imdb_categories`, `imdb_ratings`, `imdb_stars`, `length` and `mpa`) listed above.
    - A good question (a) explores relationships involving two or more variables from the data set (b) lets us use data from all (or almost all) of the films and (c) ends with a question mark.
    - As an example that fits at least (a) and (c), we might ask "Do dramas last longer than comedy films?" which could be answered using the `length` and `imdb_categories` variables, although (b) is a problem since some films are not listed as either Drama or Comedy.
    - The current version (dated 2024-09-17) of the movies data is available in our Shared Google Drive folder, or you can [download the Excel version here](https://github.com/THOMASELOVE/431-classes-2024/blob/main/movies/movies_2024-09-17.xlsx).
4. Look at this [list of films](movie_list.md). Alphabetically, what is the first film (i.e., lowest `film_id` value) that **all** of the members of your breakout group have seen? 
    - [The form](https://bit.ly/431-2024-movies-1) asks you to type in that movie's `mov_id` value and name. If there isn't a movie on the list that you've all seen, you'll type in "We couldn't find one."
5. Ensure that your group's reporter has completed [the Google Form](https://bit.ly/431-2024-movies-1) to report your group's results and has submitted the form successfully (they should receive an email confirmation.)
