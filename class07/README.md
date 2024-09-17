# 431 Class 07: 2024-09-17

[Main Website](https://thomaselove.github.io/431-2024/) | [Calendar](https://thomaselove.github.io/431-2024/calendar.html) | [Syllabus](https://thomaselove.github.io/431-syllabus-2024/) | [Text](https://thomaselove.github.io/431-book/) | [Contact Us](https://thomaselove.github.io/431-2024/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/431-data)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | get help | lab submission | for downloads

[Go here](https://thomaselove.github.io/431-2024/resources.html) for some suggested R/RStudio/Quarto learning resources.

## Today's Slides

Class | Date | Slides | Word .docx | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
07 | 2024-09-17 | **[Slides 07](https://thomaselove.github.io/431-slides-2024/class07.html)** | **[Word 07](https://thomaselove.github.io/431-slides-2024/class07w.docx)** | **[Code 07](https://github.com/THOMASELOVE/431-slides-2024/blob/main/class07.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

![](https://imgs.xkcd.com/comics/p_values.png) Source: <https://xkcd.com/1478>

## Announcements

1. I posted a revised version of the [Lab 2 instructions](https://github.com/THOMASELOVE/431-labs-2024/tree/main/lab2) on 2024-09-13 to correct a typo. The original version (in one place) suggested there were 5 tasks. There are, in fact, just 3.
    - The Lab 1 Answer Sketch was posted last Friday at noon to our Shared Google Drive.
    - **Grades** for Lab 1 will be posted by class time to our Shared Google Drive, and specifically **not** to Canvas. Look for my email dated 2024-09-16 for more details.
2. Some **Tips** for future Labs (and Projects) based on what we saw in the Lab 1 responses are [posted here](https://github.com/THOMASELOVE/431-labs-2024/blob/main/tips.md). I've also posted this next to the instructions for Labs 2-6.
3. The [Minute Paper after Class 07](https://bit.ly/431-2024-minute-07) is due Wednesday 2024-09-16 at noon.
4. Also due at noon Wednesday 2024-09-16 is [Lab 2](https://github.com/THOMASELOVE/431-labs-2024/tree/main/lab2).
5. [Chapters 9](https://thomaselove.github.io/431-book/09_moregroups.html), [10](https://thomaselove.github.io/431-book/10_transmore.html), [11](https://thomaselove.github.io/431-book/11_association.html) and [12](https://thomaselove.github.io/431-book/12_transassoc.html) of our [Course Textbook](https://thomaselove.github.io/431-book/) are now ready for you, in addition to Chapters 1-8 and the Appendix materials, which have been available previously. Chapters 13-23 still need work on my part before I can recommend you read them.
    - I also corrected non-critical irritating typos in [Section 3.5](https://thomaselove.github.io/431-book/03_summary.html#sec-outliers) and in [Section 7.5](https://thomaselove.github.io/431-book/07_transform.html#the-logarithmic-transformation) thanks to alert students who have received some credit for letting me know. Email or Campuswire is great for letting me know if you find other errors.
6. David Spiegelhalter's writing in [The Guardian](https://www.theguardian.com/profile/david-spiegelhalter) may be of interest to you.
7. Thursday September 19 is every R user's favorite holiday. I'll be sure to let you know about it next time in class.

## RStudio's Appearance

- At home, I use the following RStudio setup, which you can customize by visiting **Tools**... **Global Options** and then selecting Appearance
    - RStudio theme: Modern
    - Zoom: 125%
    - Editor font: Lucida Console
    - Editor font size: 12
    - Editor theme: Tomorrow Night Bright

## Ten More Interesting/Fun Facts about Students in this semester's 431 class

1. I can inject aesthetic Botox.
2. My family recently got a new dog named Piper.
3. I have a twin sister.
4. I speak five languages.
5. I was born in New Orleans, and enjoy cooking.
6. I used to be in the color guard in high school.
7. I have a very cute 5 month old baby.
8. I've travelled to 12 countries not including my own.
9. I've eaten ostrich and kangaroo meat before - I don't recommend either.
10. This summer, I took a road trip to Tibet and made it to the Everest Base Camp.

----------

## Favorite Movies

Consider the `movies_2024-09-17` Google Sheet now found in our Shared Google Drive. 

- This file describes **228** movies selected as a "favorite movie" by students in 431 in the Fall 2020-2024 versions of the course.
- Today, we'll describe the data gathered there gently, and talk a bit about how I developed the codebook and data, mostly using [IMDB](https://www.imdb.com/).
- In future classes, we'll augment this database in several ways, and we'll develop (and try to explore) some research questions.
- In addition to [IMDB](https://www.imdb.com/), other sites that I have used in the past to gather data about movies include:
    - <https://www.rottentomatoes.com/>, <https://www.flickchart.com/> and <https://the-numbers.com/>

## Two Last Things

1. On Sunday afternoon, I was polled (about the Ohio Senate race as well as the Presidential election) by a polling firm listed in [FiveThirtyEight's Pollster Ratings](https://projects.fivethirtyeight.com/pollster-ratings/).

2. You may be interested in [Time to Say Goodbye to the B.M.I.?](https://www.nytimes.com/2024/09/06/health/body-roundness-index-bmi.html) by Roni Caryn Rubin in the *New York Times* updated 2024-09-14.

> So welcome a new metric: the body roundness index. B.R.I. is just what it sounds like — a measure of how round or circlelike you are, using a formula that takes into account height and waist, but not weight. It’s a formula that may provide a better estimate of central obesity and abdominal fat, which are closely linked to an increased risk of developing Type 2 diabetes, hypertension and heart disease, unlike fat stored on the buttocks and thighs.

> B.R.I. scores generally run from 1 to 15; most people rank between 1 and 10. Among a nationally representative sample of 33,000 Americans, B.R.I. scores rose between 1999 and 2018, the new study found. Those with B.R.I. scores of 6.9 and up — indicating the roundest bodies — were at the highest risk of dying from cancer, heart disease and other illnesses. Their overall mortality risk was almost 50 percent greater than those with B.R.I.s of 4.5 to 5.5, which were in the midrange of the sample, while those with B.R.I. scores of 5.46 to 6.9 faced a risk that was 25 percent higher than those in the midrange.

The definition of B.R.I. used in the first paper below comes from the formula developed by [Thomas et al.](https://dx.doi.org/10.1002/oby.20408)

![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class07/bri-formula.png)

Two key articles mentioned there are:
    - [Body Roundness Index and All-Cause Mortality Among US Adults](https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2819558) from X Zhang et al. in JAMA Network Open 2024-06-05
    - [Relationships between body roundness with body fat and visceral adipose tissue emerging from a new geometrical model](https://onlinelibrary.wiley.com/doi/10.1002/oby.20408) by DM Thomas et al. in Obesity 2013-03-21, whose Figure 2, which is an example of how BRI (body roundness index) differentiates between various body types of the same BMI is reproduced below...
  
![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class07/bri-vs-bmi-fig2.jpg)

Caption: BMI as a measure of adiposity fails to distinguish individuals with similar BMI but different degrees of body fat. The three depicted individuals vary in body type but share identical BMI. A: subject is tall and lean, B: subject is muscular, C: subject has highest percent body fat. Although their BMIs are identical, their corresponding BRI values differentiate their body types. After normalizing for height, the three generated ellipses can be visually compared for differences in body roundness, which can be converted into estimates of percent body fat. Images used with permission from <http://www.shutterstock.com>. 


  

  


