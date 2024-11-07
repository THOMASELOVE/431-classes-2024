# 431 Class 20: 2024-11-07

[Main Website](https://thomaselove.github.io/431-2024/) | [Calendar](https://thomaselove.github.io/431-2024/calendar.html) | [Syllabus](https://thomaselove.github.io/431-syllabus-2024/) | [Text](https://thomaselove.github.io/431-book/) | [Contact Us](https://thomaselove.github.io/431-2024/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/431-data)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | get help | lab submission | for downloads

- Suggested [R/RStudio/Quatro learning resources](https://thomaselove.github.io/431-2024/resources.html)

## Today's Slides

Class | Date | Slides | Word .docx | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :------: | :-------------:
20 | 2024-11-07 | **[Slides 20](https://thomaselove.github.io/431-slides-2024/class20.html)** | **[Word 20](https://thomaselove.github.io/431-slides-2024/class20w.docx)** | **[Code 20](https://github.com/THOMASELOVE/431-slides-2024/blob/main/class20.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

![](https://imgs.xkcd.com/comics/probabilistic_uncertainty.png) From: https://xkcd.com/3007

## Announcements

1. I have a terrifying amount of Halloween candy to share. Please take some, by which I mean, all of it.
2. Updates on Project A feedback and grading (with a sample video and some trivia) [are here](https://github.com/THOMASELOVE/431-classes-2024/blob/main/projectA/portfolio_review.md).
3. The Project B registration form is available at <https://bit.ly/431-projB-registration-2024>. That's due next Wednesday 2024-11-13 at noon.
4. The Sample Project B materials will be posted as soon as I can finish them, but right now, Project A grading is the priority.
5. In Project B, a student asked on Campuswire about insurance groups in NHANES.
    - A problem is that you will have people who are listed as covered by multiple types of insurance, so you'll have to decide on what to do about that, since your categories need to be collectively exhaustive and mutually exclusive. I encourage you to create a four-level categorical variable for insurance type called INSURANCE as follows:
        1. If HIQ011 = No then INSURANCE = "Uninsured"
        2. If HIQ011 = Yes and HIQ032D is Yes, then INSURANCE = "Medicaid"
        3. If HIQ011 = Yes and HIQ032D is No, but HIQ032B = Yes then INSURANCE = "Medicare" (it's up to you whether you decide to treat the Medi-Gap group as part of this: see HIQ032C or not)
        4. If HIQ011 = Yes and HIQ032D and HIQ032B are both No, then if HIQ032A = Yes then INSURANCE = "Commercial" or "Private"
        5. and treat all of the subjects with HIQ011 refused or don't know, plus all of the subjects with HIQ011 = "Yes" who don't fall into the "Commercial", "Medicare" or "Medicaid" categories defined above, as missing for INSURANCE. That will leave you with not a lot of missing data, and I don't think you want to get into small groups, like you'd get with Medi-Gap or other Government Programs.
6. The bonus for using non-NHANES data in Project B is four points. I've tried to correct that now in the spot I've heard about in the [Project B instructions](https://thomaselove.github.io/431-projectB-2024/).
7. The Lab 5 answer sketch will be posted on Friday 2024-11-08 by noon.
8. R version 4.4.2 is now available, for instance at <https://cran.case.edu/>. This is very much a minor release, and I am fine with you either switching to 4.4.2, or continuing to use 4.4.1 for the remainder of this calendar year, if you choose to do so. 
9. I'd like to start incorporating at least one **standing break** into class starting today, as part of the [Stand & Move at Work Initiative](https://www.sph.umn.edu/research/projects/stand-move/) that the PQHS Department (and many other departments) are involved in here at Case. We'll see how that goes.

---

## One Last Thing

[Words Rarely Said by Academics](https://phdcomics.com/comics/archive.php?comicid=2048)

## And Then There Were None

is selling very well, but there are [still some tickets available](https://www.auroracommunitytheatre.com/) this weekend and next, if you're interested. 

## The coin flip came up "tails".

If this upsets you, you're not alone. Some things will be extra-challenging in the days (and years) to come. Try to be there for the people who will be hit harder than you, and don't be afraid to give yourself time to regroup and process the news. Please, though, don't tell me if you are happy about this.



