# 431 Class 21: 2024-11-12

[Main Website](https://thomaselove.github.io/431-2024/) | [Calendar](https://thomaselove.github.io/431-2024/calendar.html) | [Syllabus](https://thomaselove.github.io/431-syllabus-2024/) | [Text](https://thomaselove.github.io/431-book/) | [Contact Us](https://thomaselove.github.io/431-2024/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/431-data)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | get help | lab submission | for downloads

- Suggested [R/RStudio/Quatro learning resources](https://thomaselove.github.io/431-2024/resources.html)

## Today's Slides

Class | Date | Slides | Word .docx | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
21 | 2024-11-12 | **[Slides 21](https://thomaselove.github.io/431-slides-2024/class21.html)** | **[Word 21](https://thomaselove.github.io/431-slides-2024/class21w.docx)** | **[Code 21](https://github.com/THOMASELOVE/431-slides-2024/blob/main/class21.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

## An Opening Thought

![](spurious.png) 

- Note the correlation is 0.9586 for the two measures plotted above.
- Some more fun examples of the [difference between correlation and causation](http://www.tylervigen.com/spurious-correlations), from Tyler Vigen.

## Announcements

1. The Project B registration form is available at <https://bit.ly/431-projB-registration-2024>. That's due tomorrow (Wednesday 2024-11-13) at noon.
    - I hope that the Sample Study 1 and Sample Study 2 materials for Project B will be in your hands by tomorrow morning.
    - I added reminders about missing data (essentially, you use complete cases for Study 1, and imputation for missing data in Study 2) to the instructions on Sunday evening 2024-11-10 to clarify those details.
2. Also, there is a [Minute Paper](https://bit.ly/431-2024-minute-21) after today's class, due tomorrow (Wednesday 2024-11-13) at noon. The link is <https://bit.ly/431-2024-minute-21>.
3. Lab updates
    - **Lab 7**: (due 2024-12-04) Nihit Mehta was kind enough to write up some [detailed instructions for getting your Lab 7 website published to Github](https://github.com/THOMASELOVE/431-labs-2024/blob/main/lab7/lab7_publishing_advice_for_github.pdf), after following Marvin Schmitt's tutorial. See the [Lab 7 page](https://github.com/THOMASELOVE/431-labs-2024/blob/main/lab7/README.md) for more instructions, and for examples of Nihit's site and those of several other students.
    - **Lab 6**: (due 2024-11-20) Thanks to an alert student, I fixed typos in [Lab 6](https://github.com/THOMASELOVE/431-labs-2024/blob/main/lab6/README.md) where I'd inadvertently used both Lab 4 and Lab 5 when I meant Lab 6.
    - **Lab 5**: The Answer Sketch for Lab 5 is now available in our Shared Google Drive folder. Grades and feedback will be posted by the end of the day today.
4. **Project A**: Details on Project A review [are here](https://github.com/THOMASELOVE/431-classes-2024/blob/main/projectA/portfolio_review.md). Grades and feedback should be in your email **now**.
5. I've added the **gt** [package](https://gt.rstudio.com/) and the **nhanesA** [package](https://cran.r-project.org/web/packages/nhanesA/vignettes/Introducing_nhanesA.html) to the [list of suggested packages for installation](https://github.com/THOMASELOVE/431-packages). We'll see **gt** in action today.
6. **Fixing Slides 19 and 20**: I made a mistake in Slide Set 19 (slide 36, mainly) and Slide Set 20 (mainly slide 11). I have replaced the old versions of these slides (and the Word versions) for each class.
    - The mistake occurred when I fit the models `fit1`, `fit2`, and `fit3`. I should have created a new outcome `transa1c` = 100/`a1c` once I settled on a transformation before fitting the models to that outcome.
    - So, instead of fitting, for example, `lm((100/a1c) ~ a1c_old, data = dm500_i_train)`, I should instead have fit `lm(transa1c ~ a1c_old, data = dm500_i_train)`.
    - The main thing this changes is the `check_model()` result about posterior predictive checks. It doesn't affect anything we discussed in Class 19, or anything else in Class 20, but I should have done it this way throughout to demonstrate best practice, and so now I have.

## A Useful Reference

[The Science of Climate Change Explained: Facts, Evidence and Proof](https://www.nytimes.com/article/climate-change-global-warming-faq.html) by Julia Rosen in The New York Times, updated 2021-11-06.

![](climate_nyt.png)

  
## One Last Thing

from the Washington Post: "[Every voter in the US Presidential Election as a grain of sand](https://www.washingtonpost.com/elections/interactive/2024/2024-election-vote-map/?pwapi_token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJyZWFzb24iOiJnaWZ0IiwibmJmIjoxNzMxMzAxMjAwLCJpc3MiOiJzdWJzY3JpcHRpb25zIiwiZXhwIjoxNzMyNjgzNTk5LCJpYXQiOjE3MzEzMDEyMDAsImp0aSI6IjIwZWQ2YWU1LTQwYjEtNDQwNC1hNjc2LWMxNzZhMTlhNGNlOSIsInVybCI6Imh0dHBzOi8vd3d3Lndhc2hpbmd0b25wb3N0LmNvbS9lbGVjdGlvbnMvaW50ZXJhY3RpdmUvMjAyNC8yMDI0LWVsZWN0aW9uLXZvdGUtbWFwLyJ9.ON4zLEKjBGQNlm_4d9V_iGDpBaRAqgh9vMpaCJ_HUZQ&itid=gfta)" 2024-11-08.

- Thanks to [Flowing Data](https://flowingdata.com/)


