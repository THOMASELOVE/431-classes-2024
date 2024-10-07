# 431 Class 13: 2024-10-08

[Main Website](https://thomaselove.github.io/431-2024/) | [Calendar](https://thomaselove.github.io/431-2024/calendar.html) | [Syllabus](https://thomaselove.github.io/431-syllabus-2024/) | [Text](https://thomaselove.github.io/431-book/) | [Contact Us](https://thomaselove.github.io/431-2024/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/431-data)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | get help | lab submission | for downloads

- Suggested [R/RStudio/Quatro learning resources](https://thomaselove.github.io/431-2024/resources.html)

## Today's Slides

Class | Date | Slides | Word .docx | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
13 | 2024-10-08 | **[Slides 13](https://thomaselove.github.io/431-slides-2024/class13.html)** | **[Word 13](https://thomaselove.github.io/431-slides-2024/class13w.docx)** | **[Code 13](https://github.com/THOMASELOVE/431-slides-2024/blob/main/class13.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

## Announcements

1. All 42 [Project A Plans](https://github.com/THOMASELOVE/431-classes-2024/blob/main/projectA/projectA_teams.md) are accepted. Please correct any remaining issues in your [Portfolio](https://thomaselove.github.io/431-projectA-2024/portfolio.html).
    - Be sure to use the proper template for the Portfolio report, [as described here](https://thomaselove.github.io/431-projectA-2024/examples.html).
2. Grades and Feedback on Lab 3 should be posted **by class time**.
3. There is a Minute Paper after Class 13, due Wednesday 2024-10-09 at noon. **Details to come**.
4. Lab 4 is also due Wednesday 2024-10-09 at noon.
5. Quiz 1 will be in your hands by 5 PM Thursday 2024-10-10. It is due Wednesday 2024-10-16 at noon.
6. A new version (dated 2024-10-15) of the favorite movies data, incorporating [several of your suggested additions](https://github.com/THOMASELOVE/431-classes-2024/tree/main/movies#breakout-session-2), is now available at our Shared Google Drive folder.
    - New variables include information on the Bechdel-Wallace rating, Academy Awards and other award wins, budgets and revenue results from The-Numbers, rankings from Flickchart and Rotten Tomatoes, potentially triggering events from doesthedogdie, ratings of sex and nudity, violence and gore, and language, from kids-in-mind, and streaming information, along with expanded indicator variables for IMDB's top 12 genres.
    - We'll return to the movies on Tuesday 2024-10-15.

## Come see me in Agatha Christie's "And Then There Were None"!

October 25 - November 16, 2024 on Fridays and Saturdays at 7:30 PM. Tickets and more information at <https://www.auroracommunitytheatre.com/> 

## Materials Discussed in Today's Class

- Ronald L. Wasserstein, Allen L. Schirm & Nicole A. Lazar (2019) [Moving to a World Beyond "p < 0.05"](https://www.tandfonline.com/doi/full/10.1080/00031305.2019.1583913), *The American Statistician*, 73:sup1, 1-19, DOI: [10.1080/00031305.2019.1583913](https://doi.org/10.1080/00031305.2019.1583913). 
    - Ron gave a [one-hour talk you can watch here](https://t.co/GbQF01h4jU) on "[Helping to move to a world beyond p < 0.05](https://t.co/GbQF01h4jU)" which I cannot recommend enough.
- Ronald L. Wasserstein & Nicole A. Lazar (2016) [The ASA's Statement on p-Values: Context, Process, and Purpose](https://www.tandfonline.com/doi/full/10.1080/00031305.2016.1154108), *The American Statistician*, 70:2, 129-133, DOI:
[10.1080/00031305.2016.1154108](https://doi.org/10.1080/00031305.2016.1154108).
- [The Growing Importance of Reproducibility and Responsible Workflow in the Data Science and Statistics Curriculum](https://www.tandfonline.com/doi/full/10.1080/26939169.2022.2141001) by Nicholas J. Horton, Rohan Alexander, Micaela Parker, Aneta Piekut & Colin Rundel (2022) *Journal of Statistics and Data Science Education*, 30:3, 207-208, DOI: 10.1080/26939169.2022.2141001

---

Some other resources for learning more after today's talk are:

- Frank E. Harrell's [A Litany of Problems with *p*-values](https://www.fharrell.com/post/pval-litany/) blog post most recently updated in 2020.
- William Briggs' [Everything Wrong with P-values Under One Roof](http://wmbriggs.com/post/26125/) which links to a detailed article on the subject.
- Jeffrey Leek and Roger Peng [P-values are just the tip of the iceberg](references/Leek_and_Peng_2015_Pvalues_Nature.pdf)
- Jeffrey D Blume, Lucy D'Agostino McGowan, William D. Dupont, Robert A Greevy [Second-generation p values: Improved rigor, reproducibility and transparency in statistical analyses](references/Blume_etal_2018_Second_Generation_P_Values.pdf)
- Andrew Gelman and John Carlin [Beyond Power Calculations: Assessing Type S (Sign) and Type M (Magnitude) Errors](references/Gelman_Carlin_2014_Beyond_Power_Calculations.pdf)
- [Scientists rise up against statistical significance](https://www.nature.com/articles/d41586-019-00857-9) in *Nature* 2019-03-20
- [It's time to talk about ditching statistical significance](https://www.nature.com/articles/d41586-019-00874-8) also in *Nature* 2019-03-19.
- Briggs, William M., 2019. [Everything Wrong with P-Values Under One Roof](http://wmbriggs.com/post/26125/). In Beyond Traditional Probabilistic Methods in Economics, V Kreinovich, NN Thach, ND Trung, DV Thanh (eds.), pp 22–44. DOI 978-3-030-04200-4_2
- the "PROBABLE CAUSE" graphic reprinted in this [Nature piece by Regina Nuzzo](https://www.nature.com/news/scientific-method-statistical-errors-1.14700), originally from T. Sellke et al. in *The American Statistician*, 2001.
- and several great pieces by Christie Aschwanden at 538:
    - "[Not Even Scientists Can Easily Explain P-Values](https://fivethirtyeight.com/features/not-even-scientists-can-easily-explain-p-values/)", and
    - "[Statisticians Found One Thing They Can Agree On: It's Time To Stop Misusing P-values](https://fivethirtyeight.com/features/statisticians-found-one-thing-they-can-agree-on-its-time-to-stop-misusing-p-values/)", and
    - "[Science Isn't Broken](https://fivethirtyeight.com/features/science-isnt-broken/#part1)" with graphics by Ritchie King.
- You may also be interested in this piece at pbs.org about a NOVA program entitled "[Rethinking Science's Magic Number](https://www.pbs.org/wgbh/nova/article/rethinking-sciences-magic-number/)".
- I have given several talks on "Rethinking Statistical Significance" in recent years. The Github repository (90 minutes at MetroHealth Medical Center and the Center for Health Care Research and Policy, with an audio recording) is at https://github.com/THOMASELOVE/rethink, if you're a glutton for punishment.
- [Why p values are like puppies](https://www.youtube.com/watch?v=9jW9G8MO4PQ) is a 3:29 YouTube Video by Cassie Kozyrkov, MS, Chief Decision Scientist, Google Inc. It explains how to understand and interpret *p* values in an intuitive way using an example based on puppies.

## One Next-to-Last Thing

![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class13/rhodes_2022-10-02.png)

## One Last Thing

EJ Daza, [Ditch “Statistical Significance” — But Keep Statistical Evidence. How? A statistician shares a writing sample](https://towardsdatascience.com/ditch-statistical-significance-8b6532c175cb). *Towards Data Science*, 14 June 2021.
