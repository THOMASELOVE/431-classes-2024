# 431 Class 22: 2024-11-14

[Main Website](https://thomaselove.github.io/431-2024/) | [Calendar](https://thomaselove.github.io/431-2024/calendar.html) | [Syllabus](https://thomaselove.github.io/431-syllabus-2024/) | [Text](https://thomaselove.github.io/431-book/) | [Contact Us](https://thomaselove.github.io/431-2024/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/431-data)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | get help | lab submission | for downloads

- Suggested [R/RStudio/Quatro learning resources](https://thomaselove.github.io/431-2024/resources.html)

## Today's Slides

Class | Date | Slides | Word .docx | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
22 | 2024-11-14 | **[Slides 22](https://thomaselove.github.io/431-slides-2024/class22.html)** | **[Word 22](https://thomaselove.github.io/431-slides-2024/class22w.docx)** | **[Code 22](https://github.com/THOMASELOVE/431-slides-2024/blob/main/class22.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

## Announcements

1. I fixed two tiny typos (slides 25 and 27) in the [Slides for Class 18](https://github.com/THOMASELOVE/431-classes-2024/tree/main/class18). Nothing that should affect you much, but the new versions (HTML and Word) are posted. Thanks to the student who brought these to my attention.
2. [Lab 6](https://github.com/THOMASELOVE/431-labs-2024/tree/main/lab6) is due next Wednesday 2024-11-20 at noon. I revised the instructions on 2024-11-12, so make sure you have the revised version (as the changes I made should save you a lot of time in doing the Lab.)
3. **Project B**
    - The schedule for Project B Presentations [is now available](https://github.com/THOMASELOVE/431-classes-2024/blob/main/projectB/schedule.md).
    - We will walk through several issues related to the Project B plans today. My [review of the project B plans is available here](https://github.com/THOMASELOVE/431-classes-2024/blob/main/projectB/registration.md) and there is valuable stuff here for everyone, even if I've already approved your plan.
    - If your plan is [not yet approved](https://github.com/THOMASELOVE/431-classes-2024/blob/main/projectB/registration.md), then respond to my email (sent Wednesday evening 2024-11-13) to get that resolved with me as soon as possible.
4. I added two more packages, **here** and **mosaic**, to our list of [packages to install in R](https://github.com/THOMASELOVE/431-packages/blob/main/README.md). We'll demonstrate their use today.

## Our New Packages and some Nice R Resources

Recently, we've added `gt`, `nhanesA`, `mosaic` and `here` (and, less recently, `mice`) to our tool set.

- [Project MOSAIC website](https://www.mosaic-web.org/) including [R resources](https://www.mosaic-web.org/R-packages.html) and [free books on statistical thinking](https://www.mosaic-web.org/mosaic-books.html)
- The [mosaic package](https://www.mosaic-web.org/mosaic/) website, including resources describing options for [favstats()](https://www.mosaic-web.org/mosaic/reference/fav_stats.html), [df_stats()](https://search.r-project.org/CRAN/refmans/mosaicCore/html/df_stats.html) and [inspect()](https://search.r-project.org/CRAN/refmans/mosaicCore/html/inspect.html).
- The [here package](https://here.r-lib.org/) website, and Jenny Bryan's [Ode to the here package](https://github.com/jennybc/here_here)
- The [gt package](https://gt.rstudio.com/) website
- The mice (Multivariate Imputation by Chained Equations) package [reference page](https://amices.org/mice/).
- Stef van Buuren's book on multiple imputation (and mice, in particular) [Flexible Imputation of Missing Data](https://stefvanbuuren.name/fimd/)
- Heymans MW and Eekhout I [Applied Missing Data Analysis with SPSS and RStudio](https://bookdown.org/mwheymans/bookmi/)
- nhanesA [package introduction](https://cran.r-project.org/web/packages/nhanesA/vignettes/Introducing_nhanesA.html)

----

## Standing Break (at about 1:35)

- Feedback on the Minute Paper after Class 21 [is now available](https://bit.ly/431-2024-min-21-feedback). We'll discuss it during the standing break.

## Taking Other Courses With Me (repeating this from the Class 17 README)

In addition to 431, I teach two other semester-long courses, called **PQHS 432** and **PQHS 500**. I will teach both 432 and 500 in Spring 2025. Here's my advice, for what it's worth ...

- **432** is the continuation of this course (widely regarded as the "better" half.) I think **everyone** in this class should be planning to take 432 this Spring (i.e. Spring 2025), **unless** you don't feel you've received sufficient value from this course and don't need to take 432 to finish your program at CWRU, **or** you have an unshakable conflict in Spring 2025 (especially if you plan to instead take 432 in Spring 2026.)
    - I will provide the 432 website and syllabus to everyone enrolled in 432 in mid-January. The Spring 2024 syllabus for 432 is [here](https://thomaselove.github.io/432-syllabus-2024/) but of course, things will change, in ways I will start to think about after Christmas. The 432 class is held on Tuesdays and Thursdays from 1:00 to 2:15 PM.
- **500** is a project-based and more advanced course covering specific topics in the design and analysis of observational studies. 
    - I think everyone in this class who is interested in taking 500 should do so at some point. The course is mostly about using propensity scores well to help design (and analyze) data from observational studies where we want to estimate a causal effect.
    - A revised syllabus for the Spring 2025 version of the course will be available in mid-January. The Spring 2024 syllabus for 500 is [here](https://thomaselove.github.io/500-syllabus-2024/), but of course, things will change in ways I will start to think about after Christmas. The 500 course is held on Thursdays from 8:30 to 11 AM.
    - I especially think MS and PhD students (in any department) interested in applications of health research in real world situations should take it, as well as people looking for jobs in fields related to health care analytics.
    - For some people, it's better to complete 432 before taking 500 for several reasons, most especially ...
        1. percolation time for some of the ideas in 431/432
        2. too much of me at one time can be overwhelming
    - If Spring 2025 is your best opportunity to take 500, then I will certainly permit you to do so. Send me an email anytime if you want to discuss this.

## And Then There Were None

The last two performances are Friday and Satueday at 7:30. Some tickets remain available at <https://www.auroracommunitytheatre.com/>. If you come, and want to hang around for 5 minutes afterwards in the theater, the cast (including me) will come out and say hello after the play.

## One Last Thing

![](https://media.nature.com/w1248/magazine-assets/d41586-019-00857-9/d41586-019-00857-9_16546612.jpg)

Illustration by David Parkins from [Scientists rise up against statistical significance](https://www.nature.com/articles/d41586-019-00857-9) from *Nature* 2019-03-20.


