# Results of "Favorite Movies" Breakout 1

## Variables of Interest

- `imdb_stars` (weighted average star rating: 1-10)
- `imdb_ratings` (# of users who gave the movie a star rating)
- `imdb_categories` (up to 10 genre categories per movie)
- `length` (length of movie)
- `mpa` (MPA rating of movie)
- `year` (year movie was released)

## Proposed Research Questions *Verbatim*

Suggestion (*verbatim*) | Variables (*verbatim*) | Team
:---------------------------------------------- | :------------------------------ | :-:
TEL: **Do movies rated more often on IMDB have higher average ratings?** 
*Is an increase in number of IMDB star ratings related to an increase in IMDB rating?* | imdb_stars, imdb_ratings | 2
TEL: **Which movie genres have the highest average ratings?** 
*Does Sci-Fi have better weight average ratings then action?* | imdb_stars , imdb_categories  | 5
*Do sci-fi movies have higher IMDB weighted average ratings than action movies?* | imdb_stars, imdb_categories | 9
TEL: **How strong is the association of a movie's length with its average IMDB rating?** 
*Is there an association between length of movie and IMDB rating?* | imdb_stars, length  | 2
*Is there a linear relationship between length of movies (length) and IMDB ratings (imdb_stars)?* | imdb_stars, length  | 4
*Does length of movie impact the weighted IMDB star scoring?*  | imdb_stars, length  | 0
TEL: **Does the association of a movie's length with its average IMDB rating differ across genres**?
*Do romantic comedies do better, in terms of IMDB ratings, than other genres based on their length?*  | imdb_stars, imdb_categories, length  | 1
TEL: **Does the association of a movie's length with its average IMDB rating differ across MPA ratings?** 
*Is there a relationship between the length of the movie and its mpa rating with how the movie is rated in terms of its average IMDB rating.*  | imdb_stars, length, mpa  | 3
*How does MPA ratings impact imbd_stars?*  | imdb_ratings, mpa  | 8
TEL: **How strong is the association of a movie's length with its average IMDB rating?** 
*Does MPA have an effect on imdb_ratings?*  | imdb_stars, mpa  | 1 
*Do ratings (imdb_ratings) improve over time (year)? (plotting time on x-axis and ratings on y-axis in a scatterplot)* | imdb_ratings, year | 6 
TEL: **Do more recent films have higher average IMDB ratings?** 
*Is there a relationship between the year the film was released and the weighted average IMDB rating?* | imdb_stars, year | 4
*Do movies from before 2000 have a higher IMDB rating average than movies released after 2000?* | imdb_stars, year | 7
TEL: **Which movie genres have the most ratings on IMDB?** 
*Do superhero movies have a higher number of star ratings than sci-fi?* | imdb_ratings, imdb_categories  | 5
TEL: **Does the association of year and number of ratings vary by movie genre?** 
*Is there a relationship between the year a film was made and its genres with the number of star ratings according the IMDB.* | imdb_ratings, imdb_categories, year | 3
TEL: **How do movie lengths differ by their genres?** 
*Does the length of a movie differ by movie category?* | imdb_categories , length  | 6
TEL: **Do older movies have more IMDB ratings?** 
*Do older movies have more IMDB ratings?* | imdb_ratings, year | 9
*Do movies released in 2010 or before have more IMDB star ratings than movies released after 2010?*  | imdb_ratings, year | 0
TEL: **How do movie lengths differ by MPA ratings?** 
*How is the mpa rating associated with the length of a movie?* (g, pg, pg-13, R) | length, mpa | 7
TEL: **How have movie lengths changed over time?** 
*How has movie length change over the years?* | length, year  | 8

## First Movie all of you have seen from [Our List](movie1ist.md)

Team | Group | Members | First Movie on [Our List](movie1ist.md) <br /> They've All Seen
--: | :----------------: | :---: | :------------------------:
1 | Something Cool and Unique | 4 | M-001 [3 Idiots](https://www.imdb.com/title/tt1187043/)
2 | A Name You'll Remember | 6 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
3 | P B & J | 4 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
4 | Populating Pirates | 4 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
5 | The ExploreRs | 5 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
6 | The R Avengers | 5 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
7 | Tukey | 5 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
8 | Slytherin | 4 | M-012 [Back to the Future](https://www.imdb.com/title/tt0088763/)
9 | Half a dozen Pirates | 6 | M-014 [Barbie](https://www.imdb.com/title/tt1517268/)
0 | Oscars Statistician Branch | 7 | M-014 [Barbie](https://www.imdb.com/title/tt1517268/)

