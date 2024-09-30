# Favorite Movies: Breakout Activity 2

I anticipate this will take place during Class 11 (2024-10-01) or Class 12 (2024-10-03).

## Your Task(s) for Today

You'll have 25 minutes to accomplish the following tasks.

1. Form a group of 4-6 people. Come up with a name for your group that each of you will remember at our next class. If your group has fewer than 4 or more than 6 people, raise your hand, and we'll change the groups around.
2. One person in your group will report the results of your work using the Google Form found at <https://bit.ly/431-2024-movies-2>. Try to have someone who hasn't done this for prior work do this, so I can spread around the credit.
3. As a group, you will identify **two new variables** (one **categorical** and one **quantitative**) available on the internet (at least one of which should not come from IMDB) that could be added to the data to expand on what could be studied here in an interesting way. For each variable, we're hoping you will (a) identify a URL on the internet where those data seem to be available and (b) identify a **meaningful exploratory question** that incorporates that variable, along with at least one of the variables we have available in the existing data base. 
    - The current list of variables is found at the bottom of this page, and is also in the "Variable Descriptions" tab of the **movies_2024-10-01** Google Sheet in the Favorite Movies subfolder of our Shared Google Drive folder.
    - Again, at least one of the two new variables you select should come from a source other than [IMDB](https://www.imdb.com/). Two from non-IMDB sources is even better.
        - Some potential sources students have used in the past include: [Rotten Tomatoes](https://www.rottentomatoes.com/), [Flickchart](https://www.flickchart.com/), [Metacritic](https://www.metacritic.com/), [Bechdel Test Movie List](https://bechdeltest.com/), [The-Numbers](https://www.the-numbers.com/), [RogerEbert](https://www.rogerebert.com/), [Movielens](https://movielens.org/), [Filmcrave](https://www.filmcrave.com/), [Oracle of Bacon](https://oracleofbacon.org/) and [Open Movie Database](https://omdbapi.com/), but please don't feel obliged to stick to these options.
    - Your first variable should be **categorical** (with 2-10 mutually exclusive and collectively exhaustive levels, and without a lot of missing data.) 
        - An example (that you shouldn't use, since I have it already) would be the Motion Picture Association's Rating (G, PG, PG13, R, NC17 or Not Rated) which is also available on IMDB's page for the film.
        - Another example you shouldn't use is anything to do with the genre of the movie. We'll go with what we have from IMDB.
        - The categories in your suggested variable can be either ordinal or nominal.
    - The other variable you suggest should be **quantitative**, so that it takes values across a range of numerical results, and has units of measurement. 
        - An example (that you shouldn't use, since I have it already) would be the percentage of raters on IMDB that rated the film at the maximum level (10 stars) which is a percentage ranging from 0% to 100%. This is available by clicking on the number of people who rated the film on the main IMDB page.
        - In this work, we'll require a quantitative variable to be any quantity that has at minimum 11 different observed values in our set of films. Eleven is too small a count, really, to declare something "quantitative" in practice, but we'll make the best of it.
4. Ensure that your group's reporter has completed [the Google Form](https://bit.ly/431-2024-movies-2) to report your group's response and has submitted the form successfully (they should receive an email confirmation.)

## Variables Included In `movies_2024-10-01`

The current codebook for the data set called **movies_2024-10-01**, is listed below. A more detailed version is in the Variable Descriptions tab in the **movies_2024-10-01** sheet available in our Shared folder on Google Drive.

Variable | Source | Description
:---------: | :----: | -----------------------------------------------------------------------------------------------
`mov_id` | TEL | Code # (M001-M228) - alphabetical with #s first; sequels after originals
`movie` | TEL | Name of Movie
`imdb_link` | IMDB | Link to IMDB public page for movie
`year` | IMDB | Year Movie was Released
`length` | IMDB | Length of Movie (minutes)
`imdb_ratings` | IMDB | # of IMDB public ratings as of September 2024
`imdb_stars` | IMDB | # of stars (1-10) in IMDB public rating as of September 2024
`imdb_pct10` | IMDB | % of 10-star public ratings in IMDB as of September 2024
`mpa` | IMDB | Motion Picture Association rating
`director` | IMDB | Name of director(s) of film
`star_1` | IMDB | Name of first listed actor (star) in film
`gen_1` | IMDB | Gender of star_1 (M or F)
`star_2` | IMDB | Name of second listed actor (star) in film
`gen_2` | IMDB | Gender of star_2 (M or F)
`star_3` | IMDB | Name of third listed actor (star) in film
`gen_3` | IMDB | Gender of star_3 (M or F)
`metascore` | IMDB | Metascore (0-100 scale) from critic reviews at Metacritic.com
`critic_revs` | IMDB | # of critic reviews gathered at IMDB as of September 2024
`origin` | IMDB | Country (Countries) of Origin
`lang_1` | IMDB | Primary language used in the Movie
`color` | IMDB | Color or Black and White movie
`imdb_categories` | IMDB | Genre Categories (up to 10) listed by IMDB (Note: I already have indicator variables for the 12 most common genre categories.)
`imdb_synopsis` | IMDB | Synopsis from IMDB Front Page
`dr_love` | TEL | Has Dr. Love seen this movie? (Yes or No)
`mentions` | TEL | # of times movie has been mentioned by students in 431 in 2020-2024
`list_20` | TEL | # of students who mentioned this movie in the Fall 2020 version of 431
`list_21` | TEL | # of students who mentioned this movie in the Fall 2021 version of 431
`list_22` | TEL | # of students who mentioned this movie in the Fall 2022 version of 431
`list_23` | TEL | # of students who mentioned this movie in the Fall 2023 version of 431
`list_24` | TEL | # of students who mentioned this movie in the Fall 2024 version of 431

