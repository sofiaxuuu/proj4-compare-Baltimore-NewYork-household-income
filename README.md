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
![Figure 2: Average Residents Income by Parents' Income Level in Baltimore and New York](https://github.com/sophiaxuu/proj4-compare-Baltimore-NewYork-household-income/blob/main/income_by_parent_income.png)

This figure here shows the trend that the higher the parent's household income, the higher the children's household income. Also, the household income in New York is generally higher than the household income in Baltimore. 

Another finding is that for both Baltimore and New York, when comparing the average income of children with high parent income and the average income of children with middle parent income, the difference is approximately $7,000. And this difference between average income of children with middle parent income and the average income of children with low parent income is approximately $5,000.

# Business Answer 
This figure above suggests that New York has higher household income than Baltimore, MD in all parent income levels, as well as a positive relationship between children's income level and parent's income level in both cities. 

These data findings show that New York has a more robust economy than Baltimore as it has a higher average household income. To further explore why there is such a income difference, we could explore data on races, education level, employment types etc. 

# Python vs. Excel Analysis 
One advantage of Python that I find is how easily it can deal with larger dataset compared to excel. In excel, I need to scroll all the way down the file to get all data, but I don't need to deal with that in python. 
 
However, there are several inconveniences that I experience with Python. First, checking if data has a null value is harder. Previously in excel, I only need to use filter and delete empty data and you can visually see if a cell is empty, which is not possible in Python. Secondly, in python I need to be very careful with the value's datatype - I didn't realize the household income values are imported as a string rather than float number initially and it's very confusing. 

# Data Analysis Steps Description 
[Google Collaboratory Link](https://colab.research.google.com/drive/1T52BwHbq2zHpI-nfdJA0A9bxbFGCpyfh?usp=sharing)

1. Import Libraries 
2. Import datasets 
3. Filter out Baltimore and New York cities data only
4. Clean the dataset by dropping all null values 
5. Plot the Average Individual Income for residents in Baltimore vs New York figure using matplotlib 
6. Merge Baltimore and New York data to one data frame
7. Clean merged data frame by removing void values, change datatype, and rename city name 
8. Create a pivot table 
9. Plot the Average Residents Income by Parents' Income Level in Baltimore and New York figure using plotly





