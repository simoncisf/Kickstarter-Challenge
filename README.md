# Kickstarting with Excel

## Overview of Project

### Purpose

This project involves the use of statistical and analytical tools in Excel to analyze Kickstarter data for our client Louise, who is interested in starting her own Kickstarter campaign. The purpose of this project is to put in practice the tools and methods learned in the first module of this course. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

In order to understand the correlation between launch date and the outcomes of Kickstarters, we use the PivotTable tool on Excel to pull all the data we need into a table. The columns consist of outcome data, the rows are dates created, the values are outcome counts, and the table is filtered based on category and years of creation. Next, we create a Pivotchart shown below, containing the number of successful, failed, live and canceled Kickstarters for each month of the year. 

![Theater_outcomes_vs_launch](/Users/simon/Desktop/DS_Classwork/Crowdfunding_Analysis/Resources/Theater_outcomes_vs_launch.png)

### Analysis of Outcomes Based on Goals

Next, we look at the percentage of Kickstarters that were successful for a set of goal ranges. We use the countifs function in Excel to count all the Kickstarters that were successful/failed/canceled for each goal range and specifically for the subcategory of plays. Next, we calculate the percentage of those counts out of the total number of projects and plot these values against the goal ranges in the chart shown below.

![Outcomes_vs_goals](/Users/simon/Desktop/DS_Classwork/Crowdfunding_Analysis/Resources/Outcomes_vs_goals.png)

### Challenges and Difficulties Encountered

One challenge encountered in the outcomes based on goals analysis was using the countifs function to pull the correct data from the Kickstarter dataset. I initially tried filtering the outcomes column on the Kickstarter dataset such that the countifs function would only count successful or only failed campaigns, and I tried the same with the Subcategory column by filtering it to only plays. However, that did not work and I ended up adding more criteria for these columns.

## Results

Based on the Launch Date analysis, we can conclude that it is more likely that a theater campaign will be successful if it is created around the months of May and June. However, the fact that the failed campaign curve is relatively regular indicates that the spike in successful camapaigns around mid-year months might be due in part to a higher number of campaign data gathered from those months. 

Based on the Goals analysis, we can conclude that the play campaigns with goals of leass than $1000 are the most likely to succeed, as well as those in the $35000-$40000 range. This indicates that, in general, the higher the goal the more difficult it is for a campaign to succeed, which is to be expected.

These conclusions provide great insight for our client Louise, yet the dataset has some inherent limitations that reduce the reliability of such conclusions. One such limitation is the fact that there are outliers in the data that skew the data, especially when it comes to the Goals analysis because there might be unrealistically high funding goals which were never met and thus there we might be accounting for more failed campaigns than necessary.

Some other useful tables and graphs we could create would be analyzing the outcomes of theater/plays campaigns based on the number of backers and the average donation per backer, which could provide some insight into the probability of success of certain categories of campaigns or certain geographies.
