# Project B Registration Status

Unless otherwise indicated, all NHANES listings before refer exclusively to the [NHANES 2017 - March 2020 (Pre-Pandemic)](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) cycle. 

## Notes for All

1. If my listing of your project below is incorrect **in any detail**, please email me so I can fix it.
2. If your key Study 2 predictor is categorical, be sure that each category contains a substantial fraction (I would say at minimum 10%) of your available data. If not, you should collapse until it does.
3. In the instructions, I should have more actively discouraged people from using [Kaggle data sets](https://www.kaggle.com/datasets), especially those that have been pre-cleaned, and that have very limited amounts of information about how the study was designed or what the measures were. I think of these as just teaching data sets.
 
## Notes for People Using NHANES data

1. I'll remind you that NHANES provides neither a random sample, nor a representative sample (at least without weights) of the American population, so do not claim that it is either of those things.
2. Those of you using Body Mass Index as an outcome or a key predictor, consider using [Waist Circumference](https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/P_BMX.htm#BMXWAIST) instead.
3. If you were not specific, I guessed that you were planning to work with adults between the ages of 21 and 79. If that is incorrect, please email me so I can fix it.

## Friday 2024-12-06

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
1 | Alexis Heath | 9:00 AM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Blood lead | Race/Ethnicity | 6995 | Yes
2 | Tatiana Dombrovski and Mahsa Sheikh | 9:25 AM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Fasting glucose | Serum Insulin | 3616 | Yes
3 | Nihit Mehta | 9:50 AM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Body mass index | Meal skipping (3 levels) | 2112 | Yes
4 | Atticus Kenny | 2:00 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Self-reported weight | Routine access to health care (Yes or No) | 1897 | Yes
5 | Graham Stockdale | 2:25 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Serum insulin | Triglyceride | 3330 | Yes
6 | Megan Zelinsky | 2:50 PM | [Cleveland Community Cat Project Outcomes Data Set](www.communitycatproject.org/data) | Length of stay in trap-neuter-rescue/return | Intake health status (6 levels) | 444 | Yes
7 | Paul Jones | 3:15 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Body mass index | Physical activity (3 levels) | 7474 | Yes (see note)

- Paul: I would stick with adults ages 21-79, instead of 21-75 (which is what you wrote in the form), unless you have a specific reason not to do so.

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
8 | Brooke Bhattacharya and <br /> Veda Machiraju | 3:40 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Total Cholesterol | Ever drank Alcohol (Yes or No) | 2056 | Yes (see note)

- Brooke and Veda: I don't love this key predictor, since you will have very few No responses. Instead of using ALQ111, I suggest you create a multi-categorical variable using [ALQ121](https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/P_ALQ.htm#ALQ121)) which describes alcohol consumption over the past 12 months, which I would probably divide into four levels (code 0 vs. 1-4 vs. 5-7 vs. 8-10)

## Monday 2024-12-09

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
9 | Anika Krishna and Madaline Witort | 8:50 AM | National Longitudinal <br /> [Survey of Youth 1997](https://www.nlsinfo.org/content/cohorts/nlsy97/topical-guide)) | Total # of Arrests | General Health (5 levels) | 5081 | Not Yet (see note)

- Anika and Madaline: Using a count as an outcome like this (which is likely to have many, many more 0 values than anything else) requires methods for regression on count outcomes that we won't get to until well into the 432 class. A problem with many surveys of this type is that they don't provide enough quantitative variables to be useful for a linear regression project. Can you choose a better outcome?

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
10 | Saar Anis | 9:15 AM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Triglyceride | LDL Cholesterol | 4277 | OK
11 | Aishwarya Deengar and Harshita Kumar | 9:45 AM |[NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Body mass index | Urine Lead level | 2516 | Yes (see note)

- Aishwarya and Harshita: Those of you using Body Mass Index as an outcome or a predictor, consider using [Waist Circumference](https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/P_BMX.htm#BMXWAIST) instead. Not sure why you'd use lead levels from urine (URXUPB) (which I think is only available as a limited access data set anyway) instead of serum lead levels, as in [variable LBXBPB](https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/P_PBCD.htm#LBXBPB).

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
12 | Dana Jian | 10:10 AM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Minutes Sedentary per day | Ratio of Family Income to Poverty | 6830 | Yes (see note)

- Dana: The distribution of [PAD680](https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/P_PAQ.htm#PAD680) (your outcome) is highly discrete, which may wind up being frustrating for you as an outcome. Also the key predictor has a very pronounced ceiling effect, enough that it, too, may make your life very complicated.
- On the left is a histogram of the sedentary minutes per day to make my point about its discreteness. More than 90% of the 9610 values available for that variable (after you get rid of the missingness and refused codes) are one of just 10 numbers: (60, 120, 180, 240, 300, 360, 420, 480, 600 or 720.) On the right, we see a histogram of the INDFMPIR variable. Note the enormous number of values at 5.

![](images/PAD680.png)

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
13 | Olivia Lindberg | 10:35 AM | US Well-Being and <br /> [Basic Needs Survey 2018](https://www.icpsr.umich.edu/web/ICPSR/studies/37653#) | Typical hours worked per week | Food insecurity (Yes or No) | 453 | Not Yet (see note)

- Olivia: Using an outcome like this (which is likely to have nearly all of the values be one of just a few values) isn't a good choice for a linear model. A problem with many surveys of this type is that they don't provide enough quantitative variables that actually describe a wide range of results to be useful for a linear regression project. Can you choose a better outcome?

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
14 | Nick Nazak and Rebecca Stinson | 11:00 AM | HDHI Admissions <br /> [from Kaggle](https://www.kaggle.com/datasets/ashishsahani/hospital-admissions-data) | Length of Stay in Hospital | Blood hemoglobin (3 levels) | 7789 | Not Yet (see note)

- Nick and Rebecca: While I'm not a big fan of many Kaggle data sets, this one is at least semi-reasonably documented so it might be OK. But you cannot use length of stay as an outcome (it is a censored survival outcome; a time-to-event variable, and those require tools we'll see in 432), and there's no sense in categorizing the hemoglobin levels into categories like this in your key predictor - if the data are available as a quantity, use them as a quantity. You will need to figure out what to do about the same individual having multiple "admissions" in these data. I would prefer your unit to be an individual, rather than an admission, so you'll probably wind up using the first admission for each subject with multiple admissions, which will reduce the sample size, I assume. 

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
15 | JiaWei Yu | 11:25 AM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Hours of Sleep on Workdays | Vigorous Recreation? (Yes or No) | 6623 | Yes (see note)

- JiaWei: Your outcome variable is a bit of a problem, because the data are very discrete, with only about 25 different values, of which 45% (roughly) are either 7, 8 or 9. Sleeping hours is a fine predictor, but I want to warn you that it may wind up being frustrating for you as an outcome.

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
16 | Katherine Papahadjoulos | 11:50 AM | National Surveys on <br /> [Drug Use and Health (NSDUH)](https://www.samhsa.gov/data/data-we-collect/nsduh/datafiles) | Psychological Distress Scale (0-24) | Substance use severity (4 levels) | Yes
17 | Feriel Presswalla and Alayna Rowell | 12:15 PM | Health and Retirement Study <br /> [(HRS) 2022 Core](https://hrsdata.isr.umich.edu/data-products/2022-hrs-core) | Alcoholic Drinks Per Day | Degree of Pain (3 levels) | Not Yet (see note)

- Feriel and Alyna: Using a count as an outcome like this (which is likely to have many, many more 0, 1, and 2 values than anything else and also has only 16 possible values) requires methods for regression on count outcomes that we won't get to until well into the 432 class. A problem with many surveys of this type is that they don't provide enough real quantitative variables to be useful for a linear regression project. Can you choose a better outcome? In addition, why is none (or no pain) an option in your key predictor? Is this a sample of people in pain?

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
18 | Gina Lin | 12:40 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 **with a diabetes diagnosis** | Diastolic blood pressure | Age when first told you had diabetes | 1433 | Yes (see note)

- Gina: use the actually measured diastolic blood pressure in the P_BPXO data (variable BPXODI1 would be fine) instead of the questionnaire version as your Study 2 outcome. The Age variable is a problem here because if you are 30 years old, you cannot have an age when first told you had diabetes above 30, but if you are 60 years old, you can. You may want instead to look at years since diagnosis by subtracting this key predictor from the subject's age, although that too is problematic.

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
19 | Spancer Zhou | 1:05 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | **Insufficient detail** | **Insufficient detail** | 7465 | Not Yet (see note)

- Spancer: you need to be specific about what outcome (you wrote "depression quantitative" but that's not an answer) you plan to use. Give me the specifics for the variable from the NHANES materials. Then, instead of listing a long series of predictors, you needed to specify what your **key** predictor was. If you want to use blood pressure category, OK, but you need to again specify where you will obtain this information, and tell us how many people out of your 7465 are in each level.

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
20 | Jeff Lambe and <br /> Tatchaporn Ongphichetmetha | 1:50 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | LDL Cholesterol | Food Security (4 levels) | 3068 | OK
21 | Debbie Seifert | 2:15 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Hours of Sleep on Workdays | Snoring (4 levels) | 7255 | Yes (see note)

- Debbie: Your outcome variable is a bit of a problem, because the data are very discrete, with only about 25 different values, of which 45% (roughly) are either 7, 8 or 9. Sleeping hours is a fine predictor, but I want to warn you that it may wind up being frustrating for you as an outcome.

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
22 | Sarah Cooke | 2:45 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Total cholesterol | Body mass index | 7197 | Yes
23 | Mohammad Nasirpour | 3:10 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Body mass index | 1st Systolic BP | 7029 | Yes
24 | Ajay Mahenthiran | 3:35 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 **who smoke cigarettes** | Cigarettes/day | Health (5 levels) | 1687 | Yes
25 | Shraddha Dumawat | 4:00 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adult **females** ages 21-79 | Iron Binding Capacity | Marital Status (3 levels) | 1741 | Yes
26 | Kelly Bowen | 4:25 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | Median Liver Stiffness | Waist Circumference | 2878 | Yes (see note)

- Kelly: I assume you meant waist circumference as the key predictor, as indicated here. Stick to ages 21-79 unless you have a reason not to do so, though, even though your sample size may fall.

## Tuesday 2024-12-10

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
27 | Zuhair Khan | 10:35 AM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 
28 | Haley Altadonna | 11:00 AM | (BRFSS) Behavioral Risk Factor <br /> [Surveillance System 2023](https://www.cdc.gov/brfss/annual_data/annual_2023.html) |
29 | Brooke Jurasius | 11:25 AM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 
30 | Rachel Liu | 11:50 AM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 
31 | Cassandra Lopez and Guanyu Wei | 12:15 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 
32 | Dali Nemecio | 12:40 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 
33 | Arya Patel | 1:05 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 
34 | Sonny Caradonna | 1:30 PM | [TBI Model Systems (TBIMS) National Database (NDB)](https://www.tbindsc.org/Researchers.aspx)
35 | Leia George | 1:55 PM | [Social Media Usage and Emotional Well-Being from Kaggle](https://www.kaggle.com/datasets/emirhanai/social-media-usage-and-emotional-well-being?select=train.csv)
36 | Reilly Burhanna and Jose Diz Ferre | 2:10 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 
37 | Toni Shoyinka and Isaac Zeng | 2:45 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 
38 | Derek Host | 3:10 PM  | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 
39 | Tom Kupferer | 3:35 PM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 

## Wednesday 2024-12-11

Group | Investigator(s) | Start | Data Source | S2 Outcome | S2 Key <br /> Predictor | $n_{complete}$ | Approved?
:-----: | :-------------------------: | :-------: | :--------------------: | :-------: | :-------: | -------: | :----: 
40 | Weiyun Liang | 10:30 AM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 
41 | Carly DaCosta and Gabrielle Davis | 10:55 AM | [NHANES](https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2017-2020) <br /> Adults ages 21-79 | 

## As Yet Unscheduled

- Morgan McLoughlin
- Monica Ghosh
