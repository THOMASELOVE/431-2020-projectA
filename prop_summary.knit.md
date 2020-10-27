---
title: "Project A Summary based on the Proposals"
---

This page was last updated: 2020-10-27 15:08:16.



# Cleaning Your Variables

Check your five variables on the lists below, or on the Google Sheet on our Shared Drive in the Examples for Project A folder called **Details and Tips for the Variables Selected for Project A**. You should find all five of your selected variables on the list. 

- If you plan to use the variable as quantitative, do what is suggested as part of your data development work, and use that version in your codebook.
- If you plan to use the variable as a categorical predictor, you can do what you've done before for that variable, unless you prefer to make a change to the original quantitative version as indicated below.

## Ratios That Need Converting

These two variables are specified as providers per population in the raw data. You will want to multiply the values by 100,000 in order to providers per 100,000 population and get more interpretable results.

Code | Variable Description
---: | ---------------------------------------------
v004 |	Primary care physicians
v062 |	Mental health providers

## Demographics that need attention

Code | Variable Description | What to do?
---: | ----------- | ---------------
v001 |	Premature death	| Consider dividing by 100 to represent losses per 1000 population
v063 |	Median household income | Divide by 1000 to represent in thousands of dollars
v051 |	Population |	Either use log10(population), or divide population by 1000 to represent population in thousands.

## Variables that are Proportions should be converted to Percentages

Each of the variables listed below are proportions (between 0 and 1). Before you use them in any analyses, we encourage you strongly to multiply them by 100 in your data development (using mutate) to turn their values into percentages (between 0 and 100) and this will seriously ease the interpretation of slopes and transformations for these variables.

Code | Variable Description
---: | ---------------------------------------------
v002 |	Poor or fair health
v003 |  Uninsured adults (pick v003 or v085, but not both)
v009 |	Adult smoking
v011 |	Adult obesity
v021 |	High school graduation
v023 |	Unemployment
v024 |	Children in poverty
v037 |	Low birthweight
v049 |	Excessive drinking
v052 |	Proportion below 18 years of age
v057 |	Proportion Females
v058 |	Proportion Rural
v059 |  Proportion not proficient in English
v060 |	Diabetes prevalence
v067 |	Driving alone to work
v069 |	Some college
v070 |	Physical inactivity
v082 |	Children in single-parent households
v083 |	Limited access to healthy foods
v085 |  Uninsured (pick v003 or v085, but not both)
v122 |  Uninsured children (pick v085 or v122, but not both)
v132 |	Access to exercise opportunities
v136 |	Severe housing problems
v139 |	Food insecurity
v143 |	Insufficient sleep
v144 |  Frequent physical distress (pick v036 or v144, but not both)
v145 |  Frequent mental distress (pick v042 or v145, but not both)
v153 |	Homeownership
v155 |	Flu vaccinations

## Variables that should be OK as is

The variables listed below should be fine as they are. Most of them are ratios, although a few are averages or indexes. The main issue for these variables is correctly specifying the units of measurement (note that the indexes don't have units.)

Code | Variable Description
---: | ---------------------------------------------
v005 |	Preventable hospital stays
v014 |	Teen births
v036 |	Poor physical health days (pick v036 or v144, but not both)
v039 |	Motor vehicle crash deaths
v042 |	Poor mental health days (pick v042 or v145, but not both)
v043 |	Violent crime
v044 |	Income inequality
v045 |	Sexually transmitted infections
v125 |	Air pollution - particulate matter
v127 |	Premature age-adjusted mortality
v128 |	Child mortality
v133 |	Food environment index
v135 |	Injury deaths
v140 |	Social associations
v141 |  Residential segregation - Black/White (pick v141 or v142, not both)
v142 |  Residential segregation - non-White/White (pick v141 or v142, not both)
v147 |	Life expectancy
v148 |	Firearm fatalities
v156 |	Traffic volume
v159 |	Reading scores
v160 |	Math scores
v161 |	Suicides

# The remainder of this document is interesting, but not critical. It's sort of "trivia".



## Most Common Variable Selections

No two projects selected the same five variables.

Teams selected 56 of the 107 possible variables.

- The most common variable selected was `v063` (Median household income), selected in 23 of the 55 projects, but only once as an outcome.
- `v023` (Unemployment) is used in 14 projects (but never as the outcome)
- `v009` (Adult smoking) is used in 13 (only 2 times as the outcome)
- `v147` (Life expectancy) is also used in 13 (12 times as the outcome)
- `v042` (Poor mental health days) is used in 12 (6 times as the outcome)
- `v085` (Uninsured) is used in 10 (once as the outcome)
- Other common choices included:
    - `v011` (Adult obesity), `v139` (Food insecurity), `v143` (Insufficient sleep) and `v145` (Frequent mental distress) were each used in 9 projects,
    - `v021` (High school graduation), `v044` (Income inequality), `v049` (Excessive drinking) and `v070` (Physical inactivity) were each used in 8 projects,
    - `v001` (Premature death), `v062` (Mental health providers) and `v069` (Some college) were each used in 7
    - `v037` (Low birthweight), `v161` (Suicides) were each used in 6
    - `v002` (Poor or fair health), `v014` (Teen births), and `v043` (Violent crime) were each used in 5 projects

## Outcome

- 12 of 55 projects selected `v147` (Life expectancy) as their outcome
- 6 more selected `v001` (Premature death), and 6 also selected `v042` (Poor mental health days)
- 5 selected `v161` (Suicides)
- 4 selected `v037` (Low birthweight)
- 3 selected `v127` (Premature age-adjusted mortality)
- 2 selected `v002` (Poor or fair health), `v009` (Adult smoking), `v043` (Violent crime), and `v060` (Diabetes prevalence)
- while the other 11 projects used something no one else did.

## Most Common Quantitative Predictors

- 10 projects used `v063` (Median household income)
- 7 projects used `v049` (Excessive drinking)
- 6 projects used `v085` (Uninsured) and 6 used `v145` (Frequent mental distress)
- 5 projects used `v009` (Adult smoking), `v021` (High school graduation), `v023` (Unemployment), `v139` (Food insecurity) and `v143` (Insufficient sleep)

## Most Common Binary Predictors

- 7 of 55 projects selected `v023` (Unemployment) to use for a binary categorical predictor
- 5 used `v063` (Median household income)
- 4 used `v009` (Adult smoking) and 4 used `v011` (Adult obesity)

## Most Common Multi-Categorical Predictors

36 projects split into 3 categories, 10 into 4 and just 9 into 5.

- 7 of 55 projects chose `v063` (Median household income)
- 3 used `v043` (Violent crime), `v069` (Some college), `v139` (Food insecurity) and 3 used `v145` (Frequent mental distress)


# States Selected

We have 55 projects. 

- 26 projects use four states, 18 use 5 states, and 11 use 6 states.
- In total, we have 260 "states" in use.
- The states which we "permitted" you to use that no one chose were:
    - Kansas (104 counties), Kentucky (120), North Dakota (48), Nebraska (80) and Oklahoma (77).
- States (and DC) you were not permitted to use (because they have < 12 counties) were:
    - Connecticut (8 counties), Delaware (3), Hawaii (4), New Hampshire (10), Rhode Island (5) and Washington DC (1).
- Identical states were chosen by two different groups in two cases... 
    - Two projects use Ohio, Indiana, Michigan and Pennsylvania (330 counties, 4 states) 
    - Two projects use Ohio, Illinois, Indiana and Michigan (365 counties, 4 states)

Here's a graph of the states used at least once, excluding Ohio, which was used in all 55 projects:

<img src="prop_summary_files/figure-html/unnamed-chunk-1-1.png" width="480" />


# Titles of Your 55 Projects

My favorite title at the moment of these 55 is bolded. Tomorrow, I'll probably like one of the other ones better.

If you're considering a revision to your title, especially after you've completed the analyses and have something more substantial to say, I encourage you to think about whether you need words that appear many times in the other titles here, or whether there's a more effective way to entice your audience and stand out.

1. A Look into Ohio, Louisiana, Florida, and Vermont
2. An Exploration of the County Heath Rankings Data
3. Analysis of Adverse Mental Health Outcomes as a Reflection of Access to Mental Health Providers
4. Analysis of County-Level Health Indicators in Five US States
5. Analysis Of Math Test Scores in the U.S.
6. Analyzing the Factors for Premature Death
7. Assessing Poor Mental Health Days
8. Assessment and Comparing Suicidal Risk Factors in Ohio and Three Other States
9. Association of Air pollution with Poor Health Outcomes in Five States in the Great Lakes Region
10. Behavioral factors and their link with a life expectancy
11. Building a Predictive Model for Mental Health in Counties
12. CHR Data for Estimation of Birth Weight Outcomes
13. **Contributors to Violent Crime in 2020 U.S. Presidential Election Swing States**
14. Diabetes Prevalence in the 2020 County Health Rankings
15. Effect of Health Factors of a 20-Something Millenial on Life Expectancy
16. Examining factors potentially affecting low birthweight rates in six states
17. Exploration of Association of Social & Economic Factors with Health Behaviors in OH, CA, GA, SD and NJ
18. Exploration of factors potentially associated with premature death among the top ranked states for premature deaths plus Ohio
19. Exploring Life Expectancy in Midwestern US Counties
20. Factors Associated with Adult Smoking Prevalence in Four US States
21. Factors associated with violent crime across counties in OH, CA, CO, TN, & PA
22. Factors Contributing to Physical Inactivity
23. Five State Analysis of Premature Death Associations Using Community Health Rankings Data
24. Health Outcomes in the 2020 Presidential Race Battleground States
25. Health Status of Four US States
26. Impact of Health Factors on Life Expectancy in Rust Belt States
27. Impact of Public Health Factors on Low Birthweight
28. Influences on Life Expectancy in Counties in OH, NY, NJ, and CO
29. Interrogation health behaviors and life expectancy relationship:  evidence from four census region state candidates
30. Investigating Poor Mental Health Days in Select Rust Belt States
31. Modeling Preventable Hospitalization Rates at the County Level
32. Physical and Mental Health in the US
33. Poor Health May be Linked to Living in Disadvantaged Areas
34. Poor mental health: Predictors and Outcomes
35. Predicting Adult Obesity Rate in US Counties
36. Predicting adult smoking rates using mental, physical, and financial stress
37. Predicting Income Levels in Counties in the Midwest with Indicators of Community Wellness
38. Predicting life expectancy from health and social indicators
39. Predictors of Access to Mental Health Care in Counties in Six U.S. States
40. Predictors of health outcomes across counties in OH, MN, WA, and UT
41. Predictors of Life Expectancy
42. Predictors of poor perinatal outcomes in the American Midwest
43. Premature death rates analysis in four US states
44. Premature mortality across US states
45. Quality of Life and Premature Death
46. Relationship between County Life Expectancy and Health Behaviors
47. Sleep Duration, Motor Vehicle Deaths, Household Income and the Relation to Suicide in Five States
48. Socio-Economic Barriers Limit Access to Appropriate Health Care Coverage
49. Socioeconomic and Lifestyle Factors in Suicide Rates
50. Studying Life Expectancy as a Measure of Health Outcomes in 6 Representative States and Their Counties in the United States
51. The Association Between Dietary and Physical Health Behaviors, Socioeconomic Status and Life Expectancy Among 5 US States
52. The effect of Socio-economic factors and Health Behaviors on Life Expectancy across 5 States
53. The impact of various health and social factors in diabetes prevalence
54. The Relationship Between Measures of Despair and Premature Death in Midwestern States
55. What factors contribute to Suicide Rate

