# proj4-compare-Baltimore-NewYork-household-income

## Background
This project aims to compare household income in Baltimore (MD) and New York (NY). I choose these two cities because I attend university in Baltimore, and have visited New York most of the time as an international student. While Baltimore and New York are only 3-hours drives away and both are in a Metropolitan area, they are very different. New York's medium income is around $52,737 while Baltimore's median income is $41,819. New York housing costs are 495.4% more expensive than Baltimore housing costs. And New York's population is around 8,000,000 while Baltimore's population is around 620,000. The above data are from [2021 Compare Cities Overview: Baltimore, MD vs New York, NY](https://www.bestplaces.net/compare-cities/baltimore_md/new_york_ny/overview).

In particular, I want to dive into the comparison of the household income in Baltimore and New York. Since household income and socioeconomic status (SES) are key factors affecting the economic robustness of a city, I would also like to investigate how household income is affected by the income level of the previous generation. 

The dataset I used for this study is from the [Opportunity Insight Project](https://www.opportunityatlas.org/), which is a project with a mission is to identify barriers to economic opportunity and develop scalable solutions that will empower people throughout the United States to rise out of poverty and achieve better life outcomes.
 
## Business Question 
_Which city between Baltimore and New York has a more robust economy?_

## Data Question 
1. What is the average household income in Baltimore vs New York?
2. How may parent's household income affect children's household income?

## List of Data Source 
I obtain my data source all from the same website . And attached are links to my source cvs files: 
- Dataset of residents' household income in [Baltimore, MD](https://github.com/sophiaxuu/proj4-compare-Baltimore-NewYork-household-income/blob/main/baltimore_all_parent_income_rP_gP_pall.csv) and [New York, NY](https://github.com/sophiaxuu/proj4-compare-Baltimore-NewYork-household-income/blob/main/ny_all_parent_income_rP_gP_pall.csv)
- Dataset of residents' household income given parents' income is at top 25% percentile in [Baltimore, MD](https://github.com/sophiaxuu/proj4-compare-Baltimore-NewYork-household-income/blob/main/baltimore_high_parent_income_rP_gP_p75.csv) and [New York](https://github.com/sophiaxuu/proj4-compare-Baltimore-NewYork-household-income/blob/main/ny_high_parent_income_rP_gP_p75.csv).
- Dataset of residents' household income given parents' income is at top 50% percentile in [Baltimore, MD](https://github.com/sophiaxuu/proj4-compare-Baltimore-NewYork-household-income/blob/main/baltimore_middle_parent_incomerP_gP_p50.csv) and [New York](https://github.com/sophiaxuu/proj4-compare-Baltimore-NewYork-household-income/blob/main/ny_middle_parent_income_rP_gP_p50.csv).
- Dataset of residents' household income given parents' income is at top 25% percentile in [Baltimore, MD](https://github.com/sophiaxuu/proj4-compare-Baltimore-NewYork-household-income/blob/main/baltimore_low_parent_income_rP_gP_p25.csv) and [New York](https://github.com/sophiaxuu/proj4-compare-Baltimore-NewYork-household-income/blob/main/ny_low_parent_income_rP_gP_p25.csv). 

### 1. What is the average household income in Baltimore vs New York?
![Figure 1: Average Individual Income in Baltimore vs New York](https://github.com/sophiaxuu/proj4-compare-Baltimore-NewYork-household-income/blob/main/avg_indi_income_comparison.png)

This figure shows the Average Household income for Baltimore and New York. We can see there is a pretty significent gap of around $10,000 between average income in two cities, indicating that New York have a more robust economy. 

### 2. How may parent's household income affect children's household income?
[Figure 2: Average Residents Income by Parents' Income Level in Baltimore and New York](https://github.com/sophiaxuu/proj4-compare-Baltimore-NewYork-household-income/blob/main/income_by_parent_income.html)






