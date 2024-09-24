# Project A Plan Checklist for Fall 2024

## Our 17 Review Elements for Project A Plan

What will we look for in order to ACCEPT the Project A Plan, rather than require a REDO? **17 things**.

- See [the Sample Plan for an example](https://rpubs.com/TELOVE/ProjectA-sample-plan-431-2024) of what we're looking for, as needed.

### Element A. The complete Project A Plan is submitted on time.

1. On time for this evaluation was Noon on 2023-10-03. If it's more than one hour late, it will be reviewed later than those received on time, and penalized at least three points out of the 20 available.
2. If you worked with a partner, both names are shown as authors in the HTML. Exactly one of you has submitted the materials to Canvas, while the other partner has submitted a text document (Word or PDF is fine) to Canvas that reads: "My name is [YOUR NAME]. I am working on Project A with [INSERT FULL NAME OF YOUR PARTNER], and they will submit the materials for the Plan."
3. The R data set (analytic tibble), Quarto (.qmd) file, and HTML result are all present in the submission to Canvas.
4. The Quarto file produces the HTML file without errors when we run it. (Note: warnings or messages are OK, but it has to work.)

### Element B. Template, Title, Author(s) and Date show we want to see in the HTML.

1. There is a real title that does not include "Project", "Plan", "Project A" or "431" in it, but is correctly spelled, and fits in the available space in the HTML.
2. The title is no more than 80 characters in length, excluding any subtitles.
3. The title (without the subtitle) describes the work effectively on its own.
4. The author(s) name(s) appears in the HTML correctly.
5. The date is properly formatted (as, for instance, 2024-09-24) under the word PUBLISHED or MODIFIED in the HTML.
6. There is a table of contents which appears in the HTML and has exactly 14 sections, whose names match those used in the Project A Plan Template. 

### Element C. (Plan Section 1. R Packages)

1. The janitor, naniar, easystats and tidyverse packages and perhaps other packages are loaded with `library()` as part of section 1, with the tidyverse loaded last.
2. No packages in the core tidyverse (all of which load with library(tidyverse)) are loaded separately. The core tidyverse packages are dplyr, ggplot2, tidyr, readr, purrr, tibble, stringr and forcats.
3. No package is loaded more than once.
4. No package is loaded outside of Section 1.
5. `#| message: false` is used in the code chunk for Section 1 so that all messages associated with package loading are silenced.

### Element D (Plan Section 2. Data Ingest)

1. The data should be ingested into `chr_2024_raw` using `read_csv()` and thus creating a tibble, while eliminating the correct row, as described in [Data Task 1 from the Data page](https://thomaselove.github.io/431-projectA-2024/data.html#data-task-1.-ingest-the-raw-data).
2. No non-tibble data frame should ever be printed in Project A. 
3. No tibble should be printed anywhere other than in [Plan Section 9](https://thomaselove.github.io/431-projectA-2024/plan.html#section-9.-print-the-tibble).
4. The `chr_2024_raw` tibble is then filtered to the ranked counties properly, and the resulting tibble should display 3088 rows and 90 columns (we suggest using the dim() function to verify that this is true.)

### Element E (Plan Section 3: State Selection)

1. The six states selected are clearly indicated by postal abbreviation code and name, following the instructions in [Data Task 2](https://thomaselove.github.io/431-projectA-2024/data.html#data-task-2.-select-six-states).
2. There is a clear English sentence (or two) describing why you selected the states you selected.
3. You then filter the tibble to include only the ranked counties from your six states, and you demonstrate that this leads to a total number of counties between 300 and 800. (This should be demonstrated in code, and with a sentence.)
4. No counties are dropped from the states you selected.

### Element F (Plan Section 4: Variable Selection)

1. You have followed the instructions in [Data Task 3](https://thomaselove.github.io/431-projectA-2024/data.html#data-task-3.-select-analytic-variables) to develop code that identifies and selects nine variables, including the four that are required (fipscode, county, state and county_ranked), and five more (each of which are different) that you have selected.
2. All five of your selected variables are permitted for the use you're making of them, as specified in [Data Task 3 Table B](https://thomaselove.github.io/431-projectA-2024/data.html#table-b.-variables-you-can-select).
3. You have clearly identified which variables you are selecting (in a sentence, not just code) in Section 4.

### Element G (Plan Section 5: Variable Cleaning and Renaming)

1. You have followed the instructions in [Data Task 3](https://thomaselove.github.io/431-projectA-2024/data.html#clean-and-rename-your-selected-variables) to complete appropriate cleaning of each variable that needs it, and replacement of the initial versions of these variables with your cleaned alternative.
2. You have clearly indicated in Section 5 what role each outcome will play, and its initial name (from CHR 2024) along with its new name and description. (https://rpubs.com/TELOVE/ProjectA-sample-plan-431-2024).
3. You have clearly indicated what your code is doing in this section, in an English sentence or two. See [the Sample Plan for an example](https://rpubs.com/TELOVE/ProjectA-sample-plan-431-2024).

### Element H (Plan Section 6: Creating the Analysis 2 Predictor)

1. You have followed the instructions in [Data Task 4](https://thomaselove.github.io/431-projectA-2024/data.html#data-task-4.-create-a-factor-for-the-analysis-2-predictor) to develop the binary factor you will use as your Analysis 2 predictor.
2. You have clearly identified the variable being used, and described the exact cutpoints you used to create the low and high groups in one or two complete English sentences.
3. You demonstrate using code that approximately 40% of your observations are in the low group and 40% are in the high group, with missing results for the middle 20%. 

### Element I (Plan Section 7: Adding CHR 2019 Data for the Analysis 3 Outcome)

1. You have followed the instructions in [Data Task 5](https://thomaselove.github.io/431-projectA-2024/data.html#data-task-5.-add-data-from-chr-2019-for-your-analysis-3-outcome) to include the 2019 version of your Analysis 3 outcome in your tibble.
2. You have used left_join() to join the files.
3. You have renamed the two variables (2024 version and 2019 version) appropriately.
4. You have one or more complete English sentences describing what your code is doing.

### Element J (Plan Section 8: Arranging and Saving the Analytic Tibble)

1. You have arranged the variables in the order specified in [Data Task 6](https://thomaselove.github.io/431-projectA-2024/data.html#data-task-6.-re-order-variables-and-save-the-final-chr_2024-tibble).
2. The resulting Rds file is saved to a file called `chr_2024_YOURNAME.Rds` where your name is substituted in for YOURNAME, and which is part of your Canvas submission.
3. You make no changes to the tibble after Section 8.

### Element K (Plan Section 9: Print the Tibble)

1. You print the tibble by typing in chr_2024, with no other code.
2. The resulting tibble is a tibble which shows the first 10 rows, and appropriate labels for your columns.
3. The types of variables listed should match our expectations, specifically: `fipscode` and `county` are character variables, `state` and your Analysis 2 binary predictor are factors, and the other 7 variables are numeric (double-precision).

### Element L (Plan Section 10: Numerical Summaries)

1. In section 10.1, you've run code successfully to do [what is asked of you](https://thomaselove.github.io/431-projectA-2024/plan.html#section-10.1-table-of-states-by-binary-factor) (Table of States by Binary Factor). In particular, you've used `tabyl()` properly, and show row and column marginal totals, including for missing values of your binary predictor. Explanatory text is welcome but not required in this section.
2. In section 10.2, you've run `describe_distribution()` properly on the entire tibble, [as asked of you](https://thomaselove.github.io/431-projectA-2024/plan.html#section-10.2-describe_distribution-results). Explanatory text is welcome but not required in this section.
3. In section 10.3, you've run `data_codebook()` properly on the whole data set, using the settings `max_values = 6, range_at = 15)` without any errors or warnings happening, [as requested](https://thomaselove.github.io/431-projectA-2024/plan.html#section-10.3-data_codebook-results). You then include at least one English sentence to verify the issues described there, specifically regarding whether the minimum and maximum values of the quantitative data elements make sense, and that the amount of missingness meets [our requirements](https://thomaselove.github.io/431-projectA-2024/plan.html#section-10.3-data_codebook-results) for each variable.
4. In section 10.4, you've provided counts of distinct values, [as requested](https://thomaselove.github.io/431-projectA-2024/plan.html#section-10.4-distinct-values) and we can see the results for all eleven variables. You also have a sentence or two showing that the checks of distinct `fipscodes` and at least 15 unique values for each of the outcomes and the quantitative predictor exist.

### Element M (Plan Section 11: The Codebook)

1. You have a sentence stating the number of counties (should be 300-800) and variables (should be eleven) in your tibble. If we use the dim() function, we should get the same answer you did.
2. You have an attractively formatted, readable codebook that looks nice in your HTML which contains all five required parts for each of the 11 variables in your data, [as specified](https://thomaselove.github.io/431-projectA-2024/plan.html#section-11.-the-codebook). The five required columns of the table are the variable's (1) name in your tibble, (2) its role, (3) its original vXXX code, (4) the definition (including units) and (5) the year(s) in which the variable was measured.

### Element N (Plan Section 12: Research Questions)

1. You have carefully followed the detailed advice provided in [Section 12 of the Plan Instructions](https://thomaselove.github.io/431-projectA-2024/plan.html#section-12.-your-research-questions).
2. For each of the three Analyses, you provide a clear research question which is written using appropriate syntax and grammar and **ends with a question mark**.
3. Your proposed research question for each Analysis matches the task for that Analysis.
4. You have included a statement about your pre-data analysis belief about what will happen for Analysis 1, at least.

### Element O (Plan Section 13: Plan Reflection)

1. Your reflection is a paragraph describing the most challenging (or difficult) part of completing the work so far, and how you were able to overcome whatever it was that was most challenging.
2. Your paragraph is written in strong and clear English sentences, with attention paid to grammar, syntax and spelling. 
3. It is clear to us from reading the reflection what your biggest issue was, and how you tried to address it.

### Element P (Plan Section 14: Session Information)

1. We would prefer that this indicates that R version 4.4.1. is used. If you cannot use R 4.4.1, you should describe a meaningful reason to us here.
2. We’re OK with either the xfun or sessioninfo package’s session information function.

### Element Q (Spelling, Typos, Grammar)

There are no more than 2 spelling, typographical or grammatical errors in the document as a whole that we catch. Please run a spell check by hitting F7 on your Quarto before rendering it a final time, and then look at your HTML file to see if any of the headings, graphs or other elements look strange or don’t show up.

## Grading: ACCEPT or REDO

Dr. Love and the TAs will review your Plan as quickly as possible and either ACCEPT it or ask for a REDO.

ACCEPT means you’re done, and should move on the rest of Project A, perhaps while making some small changes that we request of you in your submission on Canvas.

- To receive an ACCEPT, you must meet the [Project A Plan specifications listed here](https://thomaselove.github.io/431-projectA-2024/plan.html), and pass through the 17-element review procedure listed above.

REDO means you’ll need to fix the problems we’ve identified (plus make sure you’ve done all of the 17 elements that we're checking in the review procedure) and resubmit by the deadline we give you, which will require a rapid turnaround.

## Review Procedure

For the first attempt, the TAs and Dr. Love will review the **17** elements listed above and identify each as either successfully completed or not successfully completed. 

- If a project has not successfully completed more than two of the 17 elements, we will tell you which elements (from the list of 17 above) were not successfully completed, and require a REDO before Dr. Love takes a look at the complete plan.
- If a project has not successfully completed 0, 1 or 2 of the elements below, Dr. Love will briefly review the entire Project A Plan and make a final ACCEPT or REDO decision.

For the second (and any additional) attempts, Dr. Love will review the entire Plan to ensure that it now meets the standard, including but not limited to all issues previously identified when the REDO was requested. 

- If your Plan is accepted on the initial submission and was on time, you’ll receive 20 points.
- If your Plan is accepted on the first REDO (submission 2), you’ll receive 18 points out of a possible 20.
- If your Plan is accepted on the second or third REDO (submissions 3 or 4) or later, you’ll receive 16 points out of a possible 20.
- We hope we won’t have to go further than 2 revisions for anyone.

If you don’t have some feature that we "prefer" but doesn’t alone require a REDO, we may mention this in our ACCEPT feedback and ask you to fix it in your Project A Portfolio.

- See [the Sample Plan for an example](https://rpubs.com/TELOVE/ProjectA-sample-plan-431-2024) of what we're looking for, as needed
 
