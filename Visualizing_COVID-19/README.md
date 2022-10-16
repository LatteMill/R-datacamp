# R-datacamp
My learning R language

## Task 1: Instructions
Load the readr, ggplot2, and dplyr packages.
Read in datasets/confirmed_cases_worldwide.csv using read_csv() and assign it to the variable confirmed_cases_worldwide.
Good to know
This project uses concepts found in the following courses.

Lots of plotting, including log-transforming scales and annotating plots, as covered in Introduction to Data Visualization with ggplot2 and Intermediate Data Visualization with ggplot2.
Simple manipulation of data frames, as covered in Data Manipulation with dplyr.
Reading datasets from CSV files, as covered in Introduction to Importing Data in R.
Helpful links:

tidyverse cheat sheet.
library() function documentation.
readr's read_csv() function documentation.
Importing data using read_csv() is covered in Introduction to Importing Data in R Chapter 2, Exercise 2.

## Task 2: Instructions
Using confirmed_cases_worldwide, draw a ggplot with aesthetics cum_cases (y-axis) versus date (x-axis).
Make it a line plot by adding a line geometry.
Set the y-axis label to "Cumulative confirmed cases".
Helpful links:

ggplot2's geom_line() function documentation.
ggplot2's ylab() function documentation.
Drawing single line plots is covered in Introduction to Data Visualization with ggplot2 Chapter 3, Exercise 14.
Setting axis labels is covered in Introduction to Data Visualization with ggplot2 Chapter 2, Exercise 11.

## Task 3: Instructions
Read in the dataset for confirmed cases in China and the rest of the world from datasets/confirmed_cases_china_vs_world.csv, assigning to confirmed_cases_china_vs_world.
Use glimpse() to explore the structure of confirmed_cases_china_vs_world.
Draw a ggplot of confirmed_cases_china_vs_world, assigning to plt_cum_confirmed_cases_china_vs_world.
Add a line layer. Add aesthetics within this layer: date on the x-axis, cum_cases on the y-axis, then color the lines by is_china.
Helpful links:

readr's read_csv() function documentation.
tibble's glimpse() function documentation.
ggplot2's geom_line() function documentation.
Importing data using read_csv() is covered in Introduction to Importing Data in R Chapter 2, Exercise 2.
Drawing multiple lines is covered in Introduction to Data Visualization with ggplot2 Chapter 3, Exercise 15.
Adding aesthetics to a geometry is covered in Introduction to Data Visualization with ggplot2 Chapter 1, Exercise 11.

## Task 4: Instructions
A dataset of World Health Organization events , who_events is provided. Modify the plot plt_cum_confirmed_cases_china_vs_world as follows.

Add a vertical line layer with the xintercept aesthetic mapped to date. Use the who_events data, and make it a dashed line.
Add a text layer with x mapped to date and label mapped to event. Place the labels at 100000 on the y-axis. Use the who_events data again.
Helpful links:

geom_vline() function documentation.
geom_text() function documentation.
Using geom_vline() for vertical lines is covered in Introduction to Data Visualization with ggplot2 Chapter 4, Exercise 12.
Setting the data argument to a geometry is covered in the video Introduction to Data Visualization with ggplot2 Chapter 2, Exercise 1, around 1:30.
Setting the linetype is covered (in the context of changing themes) in Introduction to Data Visualization with ggplot2 Chapter 4, Exercise 3.
Using geom_text() for vertical lines is covered in Introduction to Data Visualization with ggplot2 Chapter 4, Exercise 11.

## Task 5: Instructions
Filter rows of confirmed_cases_china_vs_world for observations of China where the date is greater than or equal to "2020-02-15", assigning to china_after_feb15.
Using china_after_feb15, draw a line plot of cum_cases versus date.
Add a smooth trend line, calculated using the linear regression method, without the standard error ribbon.
Helpful links:

dplyr's filter() function documentation.
ggplot2's geom_smooth() function documentation.
Filtering data frames is covered in Data Manipulation with dplyr Chapter 1, Exercise 6.
Adding smooth trend lines is covered in Intermediate Data Visualization with ggplot2 Chapter 1, Exercise 2.

## Task 6: Instructions
Filter rows of confirmed_cases_china_vs_world for observations of Not China, assigning to not_china.
Using not_china, draw a line plot of cum_cases versus date, assigning to plt_not_china_trend_lin.
Add a smooth trend line, calculated using the linear regression method, without the standard error ribbon.
Helpful links:

dplyr's filter() function documentation.
ggplot2's geom_smooth() function documentation.
Filtering data frames is covered in Data Manipulation with dplyr Chapter 1, Exercise 6.
Adding smooth trend lines is covered in Intermediate Data Visualization with ggplot2 Chapter 1, Exercise 2.

## Task 7: Instructions
Modify the plot, plt_not_china_trend_lin, to use a logarithmic scale on the y-axis.
Helpful links:

scale_y_log10() function documentation.
Logarithmic axis scales are covered in Intermediate Data Visualization with ggplot2 Chapter 2, Exercise 7.

## Task 8: Instructions
Code to import data on confirmed cases by country is provided. Chinese data has been excluded to focus on the rest of the world.

Look at the output of glimpse() to see the structure of confirmed_cases_by_country.
Using confirmed_cases_by_country, group by country.
Summarize to calculate total_cases as the maximum value of cum_cases.
Get the top seven rows by total_cases.
Helpful links:

dplyr's group_by() function documentation.
dplyr's summarize() function documentation.
dplyr's top_n() function documentation.
Calculating summary statistics with summarize() is covered in Data Manipulation with dplyr Chapter 2, Exercise 6.
Combining group_by() with summarize() is covered in Data Manipulation with dplyr Chapter 2, Exercise 7.
Getting the top N results is covered in Data Manipulation with dplyr Chapter 2, Exercise 10.
Using all three functions together is covered in Data Manipulation with dplyr Chapter 2, Exercise 12.

## Task 9: Instructions
Read in the dataset for confirmed cases in China and the rest of the world from datasets/confirmed_cases_top7_outside_china.csv, assigning to confirmed_cases_top7_outside_china.
Use glimpse() to explore the structure of confirmed_cases_top7_outside_china.
Using confirmed_cases_top7_outside_china, draw a line plot of cum_cases versus date, colored by country.
Set the y-axis label to "Cumulative confirmed cases".
Helpful links:

readr's read_csv() function documentation.
tibble's glimpse() function documentation.
ggplot2's geom_line() function documentation.
Importing data using read_csv() is covered in Introduction to Importing Data in R Chapter 2, Exercise 2.
Drawing multiple lines is covered in Introduction to Data Visualization with ggplot2 Chapter 3, Exercise 15.
Setting axis labels is covered in Introduction to Data Visualization with ggplot2 Chapter 2, Exercise 11.
