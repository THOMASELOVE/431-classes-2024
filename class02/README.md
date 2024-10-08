# 431 Class 02: 2024-08-29

[Main Website](https://thomaselove.github.io/431-2024/) | [Calendar](https://thomaselove.github.io/431-2024/calendar.html) | [Syllabus](https://thomaselove.github.io/431-syllabus-2024/) | [Text](https://thomaselove.github.io/431-book/) | [Contact Us](https://thomaselove.github.io/431-2024/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/431-data)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | get help | lab submission | for downloads

At the start of class today, before I turn on the Zoom recording, I'll try again to show those in attendance [Hans Rosling's 200 Countries, 200 Years, 4 minutes](https://www.youtube.com/watch?v=jbkSRLYSojo) from the BBC's *Joy of Stats*. If I fail, take a look at it in your "free time" this weekend.

## Today's Opener: The Quick Survey

As you come in, **please take** (from the box at the back table) a paper survey with 15 questions. Please read these instructions carefully before writing anything down.

1. Introduce yourself to someone near you.
2. Record the survey answers **for that other person**, while they record your responses.
3. Be sure to complete all 15 questions (both sides of the paper).
4. When you are finished, thank your partner and raise your hand. Someone will come around to collect your survey.

There is a [PDF copy of the Quick Survey here](431_surveyhandout_1perstudent_2024-08-29.pdf), if you'd like to look at the form after your paper copy has been collected.

## Today's Slides

Class | Date | Slides | Word .docx | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
02 | 2024-08-29 | **[Slides 02](https://thomaselove.github.io/431-slides-2024/class02.html)** | **[Word 02](https://thomaselove.github.io/431-slides-2024/class02w.docx)** | **[Code 02](https://github.com/THOMASELOVE/431-slides-2024/blob/main/class02.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

- The HTML link provides the (RevealJS) version of the slides that I suggest you focus on during class.
- The Word link will let you download the material in the slides as a Word (.docx) document.
    - Some people prefer this to the HTML version for live note-taking.
- The Quarto file link provides the code I used (in [Quarto](https://quarto.org/)) to build the slides. Hit the download button after clicking the link above if you want the `.qmd` file.
- To print RevealJS slides **to pdf**, [follow these instructions](https://quarto.org/docs/presentations/revealjs/presenting.html#print-to-pdf) using Google Chrome as your browser.
- We attempt to record **most** 431 classes via Zoom and post the recording to Canvas.

## Announcements

1. TAs refers to Teaching Assistants. TA Office Hours start Tuesday 2024-09-03. Our Shared Google Drive (431 Fall 2024 Dr Love and Students) contains Zoom links for these sessions in a document called **TA office hours schedule and Zoom links**, and this information is also posted to Canvas, Campuswire, and our [Contact Us](https://thomaselove.github.io/431-2024/contact.html) and [Calendar](https://thomaselove.github.io/431-2024/calendar.html) pages.
2. If there's anyone in the room today who is **not yet enrolled** in the course, see me after class. Thank you.
3. Thank you to Alayna Rowell, Feriel Presswalla, Haley Altadonna, Harshita Kumar, Jeff Lambe, Kayla Klatt, Megan Zelinsky, Nick Nazak, Toni Shoyinka, Olivia Lindberg, Sarah Cooke, Veda Machiraju, and Zuhair Khan for filling out the google form for the age guessing activity in Class 01. I appreciate the help.
4. We'll take a few minutes today to:
    - look over the [Calendar](https://thomaselove.github.io/431-2024/calendar.html) to see what's coming up,
        - Readings this weekend include Spiegelhalter through Chapter 1, [R4DS](https://r4ds.hadley.nz/): Intro and as much of "Whole game" as possible, the [Lab 1](https://github.com/THOMASELOVE/431-labs-2024/tree/main/lab1) and [Project A](https://thomaselove.github.io/431-projectA-2024/) instructions and Chapters 1-3 of [my course book](https://thomaselove.github.io/431-book/). 
    - discuss when I'll be showing R and RStudio in class, and
    - discuss how I hope you'll use [Campuswire](https://campuswire.com/) to ask and answer questions.

-------

## Welcome to 431 Survey Report

A brief report of some counts and related summaries for the Welcome to 431 Survey [is available here](welcome-report.md).

Some additional comments...

1. I speak quickly. Unfortunately, this is actually my slow speaking style you're experiencing here. I'm willing to do a lot for you, but slowing down further while speaking just isn't going to happen. That's part of the reason we try to record the sessions.
2. I'll share some interesting facts about our students in classes to come.
3. "*I am curious about your background as a researcher and statistician.*" [Syllabus description of me](https://thomaselove.github.io/431-syllabus-2024/07_professorlove.html).
4. "*What made you teach?*" Teaching is the most important thing I do for a living. My mother was a teacher, and my father was a physicist who spent most of his time working with data. I get to do both.
5. "*Where are you from?*" I was born on Long Island, in New York, and was educated at Columbia University (AB, MA, MS) and the University of Pennsylvania (MS, PhD). While I've been in Cleveland for just over 30 years, I am still a New Yorker.
6. "You seem very organized. How can I manage my time more effectively?"
    - Some food for thought from <https://www.chris-donnelly.co.uk/> ![](donnelly_time-management_2024.jpg)

## Things to Do This Weekend

1. Bookmark and familiarize yourself with the [main course website](https://thomaselove.github.io/431-2024/), being sure to visit the [Course Calendar](https://thomaselove.github.io/431-2024/calendar.html) and see what's ahead of you. You should also bookmark [R for Data Science, 2nd ed.](https://r4ds.hadley.nz/), the [R Graphics Cookbook](https://r-graphics.org/), and [Introduction to Modern Statistics, 2nd ed.](https://openintro-ims.netlify.app/), as well as the [Posit Cheat Sheets](https://posit.co/resources/cheatsheets/) page.
2. Read through the [Course Syllabus](https://thomaselove.github.io/431-syllabus-2024/).
    - Hint: I'll know on **Tuesday at 9 AM** if you've done this. Thanks to those of you who have.
3. Obtain David Spiegelhalter's *The Art of Statistics: How to Learn from Data* (~$20), and read the Introduction and Chapter 1.
    - Our [Calendar](https://thomaselove.github.io/431-2024/calendar.html) provides reading deadlines. Try to keep up.
    - Again, readings this weekend include Spiegelhalter through Chapter 1, [R4DS](https://r4ds.hadley.nz/): Intro and as much of "Whole game" as possible, the [Lab 1](https://github.com/THOMASELOVE/431-labs-2024/tree/main/lab1) and [Project A](https://thomaselove.github.io/431-projectA-2024/) instructions and Chapters 1-3 of [my course book](https://thomaselove.github.io/431-book/). 
4. [Install the software](https://thomaselove.github.io/431-2024/software.html) and [R packages, data and code](https://thomaselove.github.io/431-2024/software.html#installing-r-packages-and-datacode-for-431) you'll need.
5. **Ask us questions**. TA office hours start Tuesday, but [Campuswire is available now](https://thomaselove.github.io/431-2024/campuswire.html).

## One Last Thing

![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class02/Eivers_2024-08-10.png)  [Link to Source](https://x.com/EemerEivers/status/1822239148519890981)
