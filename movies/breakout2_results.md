# Results of "Favorite Movies" Breakout 2

## Categorical Variables

Here are the categorical variables you suggested, along with the exploratory questions you created for them...

Group | Categorical Variable | Exploratory Question
:----------: | :-----------------: | :-----------------------------------------------------------------------------------
Five Guys (We're Hungry) | [Bechdel-Wallace Test](https://bechdeltest.com/)  | Do movies that pass the Bechdel test have fewer star ratings on IMDB?
FortySixPeople | [Bechdel-Wallace Test](https://bechdeltest.com/) | How strong is the association between if a movie has passed the Bechdal Test and how often a movie has been seen by the 2024 Stats Class?
Movie HunteRs | Number of Streaming Services | Does an increased number of streaming services available also increase IMDB star rating values?
The Undecisive Statisticians | Did the movie receive an Oscar nomination? | Using a linear model, can the number of times a movie is mentioned by students in 2023-2024 predict whether or not the movie was Oscar nominated?
imdb | Did the movie receive an Oscar nomination? | Are movies with long run times more likely to be nominated for an Oscar?
"Tukey | Did the movie receive an Oscar nomination? | Is there an association between Oscar nominations and amount of money in box office ticket sales (quantitative variable)?
Something unique again  | Distributor | What is the correlation between the distributor of the movie and the imdb ratings
Sweater Weather | Franchise | Does whether a movie is made by a franchise make a difference in terms of the resulting star ratings on IMDB?

- Our `movies_2024-10-15` data now includes Bechdel-Wallace scores, information on streaming services and Academy Award ("Oscar") wins, but not nominations.
- Here is a [video explaining the Bechdel-Wallace test](https://feministfrequency.com/video/the-bechdel-test-for-women-in-movies/).
    - Bechdel-Wallace scores range from 0 to 3, and are a count of how many of these standards are met by the movie: 1. It has to have at least two named women in it. 2. Who talk to each other 3. About something besides a man. A passing score is 3, anything less doesn't pass the test.

## Quantitative Variables

Group | Quantitative Variable | Exploratory Question
:----------: | :-----------------: | :-----------------------------------------------------------------------------------
Five Guys (We're Hungry) | Box Office Gross Earnings | Do movies with a female lead (gen_1) have higher worldwide gross box office earnings (in USD)?
Tukey | Box Office Gross Earnings | Is there an association between Oscar nominations and amount of money in box office ticket sales?
Something unique again  | Box Office Gross Earnings | Does the length of the movie impact the total gross box office collection
Sweater Weather | Movie Budget | What is the association between a movie's budget and its star rating on IMDB? 
The Undecisive Statisticians  | Potentially Triggering Events | Using a linear model, can the total number of emotional trigger events in a movie predict the movie picture association rating?
FortySixPeople | Violence and Gore Rating | How strong is the association between the Violence and Gore Rating from the "Kids In Mind" report and the MPA rating?
Movie HunteRs | "Critic's Consensus" Score | Does the gender of star 1 in each movie effect the critic consensus percentage on Rotten Tomatoes?

- Our `movies_2024-10-15` data now includes several measures of a movie's box office performance, as well as its estimated budget. It also includes counts of potentially triggering events from <https://www.doesthedogdie.com/>, various ratings (0-10) from <https://kids-in-mind.com/> and various aggregated critic scores.

