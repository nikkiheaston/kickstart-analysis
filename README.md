# Kickstarting with Excel
## Overview of Project
### Purpose
The purpose of this analysis is to provide information about the outcomes of Kickstarter projects, specifically examining the time of year to launch a project, and the goal amount to be raised, within the *Theater* category and *plays* subecategory.  

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

I performed an analysis on the launch date of all Theater projects, against three possible outcomes - successful, failed, and canceled. The data dates from 2009 to 2017, and I created a pivot chart to summarize the data by month against each of the three possible outcomes. I then created a line graph to display the monthly trends for each outcome. 

![Outcomes vs Launch Date](/assets/images/Theater_Outcomes_vs_Launch.png)

From these trend lines we see that the number of successful projects is always greater than the number of failed and canceled projects. The number of canceled projects remains relatively low compared to successful and failed projects

### Analysis of Outcomes Based on Goals

I also performed an analysis on the fundraising goals for each project within the *play* subcategory and examined their outcomes. I grouped the funding goals into these dollar ranges:
- Less than 1000
- 1000 to 4999
- 5000 to 9999
- 10000 to 14999
- 15000 to 19999
- 20000 to 24999
- 25000 to 29999
- 30000 to 34999
- 35000 to 39999
- 40000 to 44999
- 45000 to 49999
- 50000 or more

I then used the COUNTIFS function in Excel to calculate the number of successful, failed, and canceled projects within each dollar range. I used the SUM function to add the total number of projects within each dollar range. Then I calculated the percentage of successful, failed, and canceled projects.

I created a line graph to dispaly the trends of each outcome across the dollar ranges. 

![Outcomes vs Goals](/assets/images/Outcomes_vs_Goals.png)

Within the *plays* subcategory there were no canceled projects, therefore the graph is an exact mirror of successful vs failed projects. 

### Challenges and Difficulties Encountered

