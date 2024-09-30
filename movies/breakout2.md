# Favorite Movies: Breakout Activity 2

I anticipate this will take place during Class 11 (2024-10-01).

## Your Task(s) for Today

You'll have 20 minutes to accomplish the following tasks.

1. Form a group of 4-6 people. Come up with a name for your group that each of you will remember at our next class. If your group has fewer than 4 or more than 6 people, raise your hand, and we'll change the groups around.
2. One person in your group will report the results of your work using the Google Form found at <https://bit.ly/431-2024-movies-2>. Try to have someone who hasn't done this for prior work do this, so I can spread around the credit.
3. As a group, you will identify **two new variables** (one **categorical** and one **quantitative**) available on the internet (not necessarily on IMDB) that could be added to the data to expand on what could be studied here in an interesting way. For each variable, we're hoping you will (a) identify a URL on the internet where those data seem to be available and (b) identify a **meaningful exploratory question** that incorporates that variable, along with at least one of the variables we have available in the existing data base. 
    - The current list of variables is [in the codebook](https://github.com/THOMASELOVE/431-classes-2024/blob/main/movies/codebook1.md) and also at the bottom of this page.
    - At least one of the two new variables you select should come from a source other than [IMDB](https://www.imdb.com/).
        - A few other potential sources: [Rotten Tomatoes](https://www.rottentomatoes.com/), [Flickchart](https://www.flickchart.com/), [Metacritic](https://www.metacritic.com/), [Bechdel Test Movie List](https://bechdeltest.com/), [The-Numbers](https://www.the-numbers.com/), [RogerEbert](https://www.rogerebert.com/), [Movielens](https://movielens.org/), [Filmcrave](https://www.filmcrave.com/), [Oracle of Bacon](https://oracleofbacon.org/) and [Open Movie Database](https://omdbapi.com/), but please don't feel obliged to stick to these options.
    - Your first variable should be **categorical** (with 2-10 mutually exclusive and collectively exhaustive levels, and without a lot of missing data.) 
        - An example (that you shouldn't use, since I have it already) would be the Motion Picture Association's Rating (G, PG, PG13, R, NC17 or Not Rated) which is also available on IMDB's page for the film.
        - Another example you shouldn't use is anything to do with the genre of the movie. We'll go with what we have from IMDB.
        - The categories in your suggested variable can be either ordinal or nominal.
    - The other variable you suggest should be **quantitative**, so that it takes values across a range of numerical results, and has units of measurement. 
        - An example (that you shouldn't use, since I have it already) would be the percentage of raters on IMDB that rated the film at the maximum level (10 stars) which is a percentage ranging from 0% to 100%. This is available by clicking on the number of people who rated the film on the main IMDB page.
        - In this work, we'll require a quantitative variable to be any quantity that has at minimum 11 different observed values in our set of films. Eleven is too small a count, really, to declare something "quantitative" in practice, but we'll make the best of it.
4. Ensure that your group's reporter has completed [the Google Form](https://bit.ly/431-2024-movies-2) to report your group's response and has submitted the form successfully (they should receive an email confirmation.)

## The Variables Included In `movies_2024-10-01`

The [current codebook is available here](https://github.com/THOMASELOVE/431-classes-2023/blob/main/movies/codebook1.md), and below for the data set called `movies_2023-09-14`, available on our Shared Drive.

Variable | Description
---------: | :---------------------------------------------------------------------------
`film_id`	| Film # (1-201) - alphabetical placing numbers first; sequels after originals
`film`	| Film's title
year	| Film's year of release
length	| Length of film in minutes
mpa	| Motion  rating (G, PG, PG-13, R, NC-17)
imdb_categories	| Up to three categories (from IMDB listing) out of 20 possibilities
star_1	| Name of first star in film
star_2	| Name of second star in film
star_3	| Name of third star in film
director	| Name of director(s) of film
imdb_ratings	| # of IMDB public ratings as of 2023-09
imdb_stars	| # of stars (0-10) in IMDB public rating as of 2023-09
imdb_pct10	| % of 10-star public ratings in IMDB as of 2023-09
imdb_link	| Link to IMDB public page for film
dr_love	| Has Dr. Love seen this film? (Yes or No)
mentions	| # of times film has been mentioned by students in 431 between 2020-2023
list_2020	| # of students who mentioned this film in the Fall 2020 version of 431
list_2021	| # of students who mentioned this film in the Fall 2021 version of 431
list_2022	| # of students who mentioned this film in the Fall 2022 version of 431
list_2023	| # of students who mentioned this film in the Fall 2023 version of 431
rt_critics | % of critics who favorably reviewed the film (via Rotten Tomatoes)
rt_audience | % of audience reviewers who were favorable about the film (via Rotten Tomatoes)

- Note that the two `rt_` variables are available in our existing file only for films mentioned by students in the Fall 2023 version of 431 in the current data, but Dr. Love has also gathered these two variables for all of the other movies.
