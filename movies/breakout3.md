# Favorite Movies: Breakout Activity 3

We will complete this task in Class 15 (2024-10-15).

## Breakout Activity 2 report

- A Brief Report on your Proposed Variables and Exploratory Questions from Breakout 2 [is available here](breakout2_results.md).
- A brief list of variable names and descriptions for the 80 variables in our `movies_2024-10-15` data [is here](codebook_2024-10-15.md). An even more complete codebook is in the *Variable Descriptions* tab of our shared Google Sheet.

## Your Task(s) for Breakout Activity 3

- Form a group of 4-6 people. Come up with a name for your group that each of you will remember at our next class. If your group has fewer than 4 or more than 6 people, raise your hand, and we'll change the groups around.
- One person in your group will report the results of your work using the Google Form found at <https://bit.ly/431-2024-movies-3>. Try to have someone who hasn't done this for prior work do this, so I can spread around the credit.
- As a group, you will go through the five steps listed below, which involve selecting four variables (at least one of which must have missing values) and which will fuel three analyses, then you will describe research questions that lead to specific comparisons using those variables, as described below. Finally, you'll pull the data into R and calculate a correlation coefficient. You might prefer to use this [downloadable .csv version](https://github.com/THOMASELOVE/431-classes-2024/blob/main/movies/movies_2024-10-15.csv) of the data in our `movies_2024-10-15` file.
- Ensure that your group's reporter has completed [the Google Form](https://bit.ly/431-2024-movies-3) to report your group's responses and has submitted the form successfully (they should receive an email confirmation.) The Google Form is found at <https://bit.ly/431-2024-movies-3>.

----------

**Step 1.** First, you will identify a comparison of a quantitative outcome (from the [outcome options list below](#outcome-options-for-step-1)) across levels of a binary predictor (from the [binary predictor options list below](#binary-predictor-options-for-step-1) that is of interest to you, and create a research question which leads directly to that comparison, is written clearly, and ends with a question mark.

**Step 2.** Next, you will identify a covariate (a quantitative predictor which should have a reasonably strong relationship with the outcome you chose in Step 1) which we could adjust for in making the comparison you developed in Step 1, and you'll then create a revised Step 1 research question to include the fact that you'll be adjusting for this covariate. 
    - The [list of available covariate options is here](#covariate-options-for-step-2).

**Step 3.** Finally, you will identify a new predictor for the comparison in Step 1, this time using a multi-categorical predictor (from the [multi-categorical predictor list below](#multi-categorical-predictor-options-for-step-3)), and you'll use this to create a Step 3 research question to use this predictor instead of the one you identified in Step 1, and the fact that you'll again be adjusting for the covariate from Step 2 in this model, while re-using the outcome from Step 1.

**Step 4.** Identify the number of missing observations in each of your four chosen variables (the outcome from Step 1, the binary predictor from Step 1, the covariate from Step 2, and the multi-categorical predictor for Step 3.) 
    - **At least one of your four variables must have at least one missing value, please.** 
    - You'll be asked about missing values as you specify each variable in the [Google Form](https://bit.ly/431-2024-movies-3).
    - The tables below specify the number of missing values in each variable listed, plus this information is also available in the Variable Descriptions tab of the Google Sheet for movies_2024-10-15 in our Shared Folder.

**Step 5.** Use R to find the Pearson correlation between your covariate (from Step 2) and your outcome (from Step 1).
    - Drop any missing values when estimating this correlation value, and specify the correlation coefficient to two decimal places.

### Outcome Options (for Step 1)

Here are the 11 options I'd like you to choose from. Pick one that you're interested in, because you'll use the same outcome throughout this work.

Variable | Description | NA (# missing)
--------: | ------------------------------------------ | ----
`imdb_pct10` | % of 10-star public ratings in IMDB as of September 2024 | 0
`metascore` | Metascore (0-100 scale) from critic reviews at Metacritic.com | 14
`awards` | # of awards (wins) according to IMDB | 0
`budget` |  Estimated Budget via IMDB (in `US$`) | 22
`gross_world` | Gross Revenue Worldwide (`US$`) | 8
`fc_no1` | Flickchart users who have movie as number 1 on their list | 1
`rt_audience` | Rotten Tomatoes Popcornmeter (% Fresh via Audience) | 1
`rt_reviews` | # of Critic Reviews gathered at Rotten Tomatoes | 0
`theaters` | Maximum number of Theaters in which the movie played | 36
`box_2023` | Inflation-Adjusted Domestic Box Office (in 2023 $) | 31
`triggers` | Number of Potentially Triggering Events (Abandonment, Abuse, etc.) | 3

### Binary Predictor Options (for Step 1)

Here's a list of seven options, and read the material below this table, as well.

Variable | Description | NA (# missing)
--------: | ------------------------------------------ | ----
`gen_1` | Gender of star_1 (M or F) | 0
`origin` | Country of Origin includes US? (Yes or No) | 0
`lang_1` | Primary language used in the Movie (English or Not English) | 0
`dr_love` | Has Dr. Love seen this movie? (Yes or No) | 0
`list_24` | did at least one 2024 student mention this movie? (Yes or No) | 0
`drama` | Is Drama one of the genres listed in imdb_categories? (1 = yes, 0 = no) | 0
`comedy` | Is Comedy one of the genres listed in imdb_categories? (1 = yes, 0 = no) | 0

- **or** you can use any quantitative variable in the [`movies_2024-10-15` data](https://github.com/THOMASELOVE/431-classes-2024/blob/main/movies/codebook_2024-10-15.md), so long as you provide a cutpoint to specify the top 40% and bottom 40% of the data, as you did in Project A. This will, naturally, create some missing values, and that is OK, but won't count as your "variable with missing data" for this activity.
- **or** you can use any multi-categorical variable in the [`movies_2024-10-15` data](https://github.com/THOMASELOVE/431-classes-2024/blob/main/movies/codebook_2024-10-15.md), so long as you specify a binary version of that variable (so which levels will be collapsed) - an example would be whether or not the `bw_rating` was 3 (passing) or not, another would be whether the movie had a value of `oscars` greater than 0 (i.e. the movie won at least one Academy Award.)

### Covariate Options (for Step 2)

Any of the variables in the outcome options list that you didn't already use, and also any of these variables:

Variable | Description | NA (# missing)
--------: | ------------------------------------------ | ----
`year` | Year Movie was Released | 0
`length` | Length of Movie (minutes) | 0
`kim_sn` | Kids-In-Mind Sex & Nudity rating (1 - 10, higher = more) | 71
`kim_vg` | Kids-In-Mind Violence & Gore rating (1 - 10, higher = more) | 71
`kim_lang` | Kids-In-Mind Language rating (1 - 10, higher = more) | 71

### Multi-Categorical Predictor Options (for Step 3)

Variable | Description | NA (# missing)
--------: | ------------------------------------------ | ----
`mpa` | Motion Picture Association rating (we'll only use PG, PG-13, R and Other) | 0
`bw_rating` | Bechdel-Wallace Test Criteria Met (0-3) | 10
`oscars` | # of Oscar (Academy Award) wins according to IMDB | 0
`ebert` | Movie Review (from Roger Ebert or other reviewer) on 1 to 4 stars scale | 29
`stream_n` | # of Streaming Services listed at Rotten Tomatoes (range: 0-5) | 0

as well as the `kim_sn`, `kim_vg`, and `kim_lang` variables added as covariate choices for Step 2, so long as you didn't use them already in Step 2.
