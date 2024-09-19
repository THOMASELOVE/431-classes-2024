# 431 Class 08: 2024-09-19

[Main Website](https://thomaselove.github.io/431-2024/) | [Calendar](https://thomaselove.github.io/431-2024/calendar.html) | [Syllabus](https://thomaselove.github.io/431-syllabus-2024/) | [Text](https://thomaselove.github.io/431-book/) | [Contact Us](https://thomaselove.github.io/431-2024/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/431-data)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | get help | lab submission | for downloads

- Suggested [R/RStudio/Quatro learning resources](https://thomaselove.github.io/431-2024/resources.html)

## Today's Slides

Class | Date | Slides | Word .docx | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
08 | 2024-09-19 | **[Slides 08](https://thomaselove.github.io/431-slides-2024/class08.html)** | **[Word 08](https://thomaselove.github.io/431-slides-2024/class08w.docx)** | **[Code 08](https://github.com/THOMASELOVE/431-slides-2024/blob/main/class08.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

## Announcements

1. Effective tonight and for the rest of the semester, Thursday TA office hours will be held from 9:00 to 10:30 PM, instead of 7:30 to 9 PM. Sorry for the change.
2. A student was good enough to point out that I've been unclear. We don't really have a Shared Google Drive, but instead a Shared Folder in your My Drive, called **431 Fall 2024 Students and Dr Love**. I am sorry about that.
3. Student Videos introducing themselves (from Lab 1, task 5) are now available for you to watch (as you like) in the **Student Introductory Videos** subfolder of our Shared Google Drive folder.
4. Feedback on the Minute Paper after Class 07 [is available now](https://bit.ly/431-2024-min-07-feedback). Grades on the 431 Student Grade Roster in our Shared Google Drive folder are up to date, as well.
    - Someone asked what you need to do to get full credit on a Minute Paper. To increase your chances, (1) get it in on time, and (2) Include something thoughtful (as a complete sentence, ideally) in your response, especially in response to the standard questions I ask every time (What was the most important thing, and what questions do you have for me.)
5. The [Lab Regrade Request Form](https://bit.ly/431-2024-lab-regrade-request) is now available. This form is **optional**, and is used solely for you to ask me to review your grade on one or more of Labs 1-6. The form is due at the end of the semester - see the [Calendar](https://thomaselove.github.io/431-2024/calendar.html) for the specific date and time.
    - Details on the Lab Regrade policy [are found here](https://github.com/THOMASELOVE/431-labs-2024/blob/main/README.md#lab-regrade-requests-will-be-reviewed-in-december). 
6. David Spiegelhalter's writing in [The Guardian](https://www.theguardian.com/profile/david-spiegelhalter) may be of interest to you.

---

## Today is [an R User's favorite holiday](https://en.wikipedia.org/wiki/International_Talk_Like_a_Pirate_Day).

-
-
-



![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class08/Sept_19_2024.png)

-
-
-


![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class08/R_keyboard.png)


## Favorite Movies

Today we'll have our [first breakout session related to the Favorite Movies data](https://github.com/THOMASELOVE/431-classes-2024/tree/main/movies).

-----

## Main Thing To Work On This Weekend?

The [Project A Plan](https://thomaselove.github.io/431-projectA-2024/plan.html), which is due Wednesday at noon.

## Self-Promotion

I'm [in a play](https://github.com/THOMASELOVE/theater/blob/master/README.md#my-next-performances-will-be-as-justice-wargrave-in-the-play-and-then-there-were-none-at-aurora-community-theatre-october-25---november-16-2024) that runs from October 25 - November 16. You'll hear more about this in October, but if you want to get tickets now, [visit this link](https://www.auroracommunitytheatre.com/). 

### If I'm a student/friend/neighbor/colleague of yours, are you expecting me to come see you in theater?

I'm always delighted to see anyone I know at any show I do. Please do come if you are interested, and comfortable being around people who are unmasked. I also have various professional roles (as a teacher, for example) where I have some nominal control over other people's happiness or work. If you're someone who interacts with me professionally, please feel no obligation to attend a show I'm in. Attending (or not attending) a show I'm in carries **no** weight with me at all in any professional capacity.

## One Last Thing

2024-09-18/2024-09-19 Presidential Election Forecasts: Snapshots

- <https://projects.fivethirtyeight.com/2024-election-forecast/> (FiveThirtyEight)

![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class08/2024-09-18/fivethirtyeight.png)

- <https://www.economist.com/interactive/us-2024-election/prediction-model/president> (The Economist)

![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class08/2024-09-18/the-economist.png)

- <https://elections2024.thehill.com/forecast/2024/president/> (Decision Desk HQ at The Hill)

![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class08/2024-09-18/decision_desk_hq.png)

- <https://projects.cnalysis.com/23-24/president> (CNalysis)

![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class08/2024-09-18/cnalysis.png)

- <https://projects.jhkforecasts.com/2024/president/#standard> (JHK Forecasts)

![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class08/2024-09-18/jhkforecasts.png)

- <https://www.racetothewh.com/president/2024> (Race To the White House)

![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class08/2024-09-18/race_to_the_white_house.png)

- <https://www.natesilver.net/p/nate-silver-2024-president-election-polls-model> (Silver Bulletin: pay wall for image shown here)

![](https://github.com/THOMASELOVE/431-classes-2024/blob/main/class08/2024-09-18/silver_bulletin.png)
