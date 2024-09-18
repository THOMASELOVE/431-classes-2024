## Favorite Movies: Breakout Activity 1

To be completed on 2023-09-21 (Class 08).

## The Five Variables We're Focusing On Today

We will use the `movies_2023-09-14` data in the `favorite_movies` directory on our Shared Drive, which describes 201 films mentioned as "favorites" by students in 431 for Fall 2020, 2021, 2022 or 2023. The data are [also found here](movies_2023-09-14.csv).

There are five variables (`year`, `length`, `imdb_categories`, `imdb_ratings`, and `imdb_stars`) that we will focus on today...

Variable | Sample Value | Explanation
:--------: | :------------: | ------------------------------------------------------------------------
`film_id` | 11 | code (1-201): arranges in alphabetical order by title, ignoring starting "The" or "A"
`film` | Avengers: Endgame | film title according to IMDB
**`year`** | 2019 | year film was released
**`length`** | 181 | length of film (in minutes)
**`imdb_categories`** | Action, Adventure, Drama | Film Categories specified by IMDB (up to 3)
**`imdb_ratings`** | 1,200,000 | Number of Star Ratings (IMDB)
**`imdb_stars`** | 8.4 | Weighted Average Rating (IMDB)

Note that some details on [the `imdb_categories` data are available to you at this link](codebook1.md#more-on-imdb_categories).

## Your Task(s) for Today

You'll have between 15 and 20 minutes to accomplish the following tasks.

1. Form a group of 4-6 people. Come up with a memorable name for your group that each of you will still remember in a week.
2. One person in your group will report the results of your work using the Google Form found at <https://bit.ly/431-2024-movies-1>. 
3. As a group, you will identify **two** exploratory questions about films in this sample that could be addressed using the five key variables (`year`, `imdb_categories`, `imdb_ratings`, `imdb_stars` and `length`) listed above.
    - A good question (a) explores relationships involving two or more variables from the data set (b) lets us use data from all (or almost all) of the films and (c) ends with a question mark.
    - As an example that fits at least (a) and (c), we might ask "Do dramas last longer than comedy films?" which could be answered using the `length` and `imdb_categories` variables, although (b) is a problem since some films are not listed as either Drama or Comedy.
    - The current version (dated 2023-09-14) of the movies data is available on our Shared Google Drive, and [also here](movies_2023-09-14.csv).
    - Here is the [full codebook that explains what the other variables in the data mean](codebook1.md) but for today, we're sticking to the five variables listed above.
4. Look at this [list of films](movie_list.md). Alphabetically, what is the first movie (i.e., lowest `mov_id` value) that **all** of the members of your breakout group have seen? 
    - [The form](https://bit.ly/431-2024-movies-1) asks you to type in that movie's `mov_id` value and name. If there isn't a movie on the list that you've all seen, you'll type in "We couldn't find one."
5. Ensure that your group's reporter has completed [the Google Form](https://bit.ly/431-2024-movies-1) to report your group's results and has submitted the form successfully (they should receive an email confirmation.)
