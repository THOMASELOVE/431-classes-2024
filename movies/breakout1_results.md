# Results of "Favorite Movies" Breakout 1

## Variables of Interest

- `imdb_stars` (weighted average star rating: 1-10)
- `imdb_ratings` (# of users who gave the movie a star rating)
- `imdb_categories` (up to 10 genre categories per movie)
- `length` (length of movie)
- `mpa` (MPA rating of movie)
- `year` (year movie was released)

## Your Research Questions and My Efforts to Clean Them Up

- Dr. Love's suggested versions of your questions are **shown in bold**.
- Questions *in italics* are taken verbatim from your submissions.
    - Major problems with genres (`imdb_categories`) are that movies can have more than one genre (and as many as 10), and there are so many of them (there are dozens of them, in fact, in our sample.)
    - MPA ratings (`mpa`), like genres, include multiple categories (really everything other than PG, PG-13 and R) with very few observations.

1. TEL suggests: **How strong is the association between how often a movie is rated on IMDB and its number of stars?** (`imdb_stars`, `imdb_ratings`)
    - *Is an increase in number of IMDB star ratings related to an increase in IMDB rating?* (I would tweak the names for clarity's sake.)
2. TEL suggests **Which movie genres have the highest average ratings?** (`imdb_stars`, `imdb_categories`)
    - *Do sci-fi movies have higher IMDB weighted average ratings than action movies?* (what do you do about movies that are listed as both Sci-Fi and Action in `imdb_categories`?
    - *Does Sci-Fi have better weight average ratings then action?* (you mean weighted, not weight)
3. TEL: **How strong is the association of a movie's length with its average IMDB rating?** (`imdb_stars`, `length`)
    - *Is there an association between length of movie and IMDB rating?* (I assume you mean `imdb_stars` here not the number of ratings)
    - *Is there a linear relationship between length of movies (length) and IMDB ratings (imdb_stars)?* (try not use ratings when you mean stars, and vice versa)
    - *Does length of movie impact the weighted IMDB star scoring?* (you're suggesting a causal inference here - I would probably avoid using impact as a verb)
4. TEL: **Does the association of a movie's length with its average IMDB rating differ across genres**? (`imdb_stars`, `length`, `imdb_categories`)
    - *Do romantic comedies do better, in terms of IMDB ratings, than other genres based on their length?* (nice try involving three variables, but the question isn't clear)
5. TEL: **Does the association of a movie's length with its average IMDB rating differ across MPA ratings?** (`imdb_stars`, `length`, `mpa`)
    - *Is there a relationship between the length of the movie and its mpa rating with how the movie is rated in terms of its average IMDB rating.*  (sure there's *a* relationship, but is it strong?, and where's your question mark?)
6. TEL: **How strong is the association of a movie's MPA rating with its average IMDB rating?** (`imdb_stars`, `mpa`)
    - *How does MPA ratings impact imbd_stars?*
    - *Does MPA have an effect on imdb_ratings?* 
7. TEL: **Do more recent films have higher average IMDB ratings?** 
    - *Do ratings (imdb_ratings) improve over time (year)? (plotting time on x-axis and ratings on y-axis in a scatterplot)* (the scatterplot description doesn't really help, and I worry about causal language a bit.)
    - *Is there a relationship between the year the film was released and the weighted average IMDB rating?* (there is always some sort of relationship - is it strong? is it linear?)
    - *Do movies from before 2000 have a higher IMDB rating average than movies released after 2000?* (OK)
8. TEL: **Which movie genres have the most ratings on IMDB?** 
    - *Do superhero movies have a higher number of star ratings than sci-fi?* (again, what about movies in both genres?)
9. TEL: **Does the association of year and number of ratings vary by movie genre?** 
    - *Is there a relationship between the year a film was made and its genres with the number of star ratings according the IMDB.* (you need the word "to" before "the IMDB" and a question mark, as well. Also, sure there's a relationship, as always.)
10. TEL: **How do movie lengths differ by their genres?** 
    - *Does the length of a movie differ by movie category?* (OK, I think, but what do we do about overlap in genres?)
11. TEL: **Do older movies have more IMDB ratings?** 
    - *Do older movies have more IMDB ratings?* (OK)
    - *Do movies released in 2010 or before have more IMDB star ratings than movies released after 2010?* (OK - a split like this could work)
12. TEL: **How do movie lengths differ by MPA ratings?** 
    - *How is the mpa rating associated with the length of a movie?* (OK)
13. TEL: **How have movie lengths changed over time?** 
    - *How has movie length change over the years?* (you want changed, not change)

## First Movie all of you have seen from [Our List](movie1ist.md)

Group | Members | First Movie on [Our List](movie1ist.md) <br /> They've All Seen
:----------------: | :---: | :------------------------:
Something Cool and Unique | 4 | M-001 [3 Idiots](https://www.imdb.com/title/tt1187043/)
A Name You'll Remember | 6 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
P B & J | 4 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
Populating Pirates | 4 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
The ExploreRs | 5 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
The R Avengers | 5 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
Tukey | 5 | M-009 [Avatar](https://www.imdb.com/title/tt0499549/)
Slytherin | 4 | M-012 [Back to the Future](https://www.imdb.com/title/tt0088763/)
Half a dozen Pirates | 6 | M-014 [Barbie](https://www.imdb.com/title/tt1517268/)
Oscars Statistician Branch | 7 | M-014 [Barbie](https://www.imdb.com/title/tt1517268/)

