# Kickstarting with Excel
## Overview of Project
### Purpose
The purpose of this analysis is to provide information about the outcomes of Kickstarter projects, specifically examining the time of year to launch a project, and the goal amount to be raised, within the *Theater* category and *plays* subecategory.  

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

I performed an analysis on the launch date of all Theater projects, against three possible outcomes - successful, failed, and canceled. The data dates from 2009 to 2017, and I organized the data into a pivot chart. The pivot chart can be filtered by Kickstarter's main categories (i.e. Theater, Food, Games, etc.) and by year. The pivot chart displays monthly data for each of the three outcomes. Using the filters I was able to compare the Theater category across the years from 2009 to 2017, and to the other categories. 

I then created a line graph to display the monthly trends for each outcome for all years. 

![Outcomes vs Launch Date](https://github.com/nikkiheaston/kickstart-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

From these trend lines we see that the number of successful projects is always greater than the number of failed and canceled projects. The number of canceled projects remains relatively low compared to successful and failed projects

### Analysis of Outcomes Based on Goals

I also performed an analysis on the fundraising goals for each project within the *plays* subcategory and examined their outcomes. I grouped the funding goals into these dollar ranges:
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

![Outcomes vs Goals](https://github.com/nikkiheaston/kickstart-analysis/blob/main/Outcomes_vs_Goals.png)

Within the *plays* subcategory there were no canceled projects, therefore the line for successful projects is an exact mirror of failed projects. 

### Challenges and Difficulties Encountered

The greatest challenge I encountered was in analyzing the Outcomes Based on Goals. I initially used the COUNTIFS function incorrectly, counting all instances of each of the successful, failed, and canceled projects, rather than drilling down to the *plays* projects. To correct this I learned how to use the COUNTIFS function, which is to use multiple arguments within the function, essentailly meaning all the criteria must be met for a cell to be counted. 

## Results

I have drawn two conclusions from the Outcomes Based on Launch Date Analysis:
1) Launching a project in the late spring through summer is best, especially during the month of May, yields the highest number of successful projects.
2) Avoid launching a project during December - there were almost as many failed projects in December as there were sucessful. 

I have also drawn two conclusions from the analysis of the Outcomes Based on Goals:
1) The majority (approx. 95%) of the successful projects raised less than $15,000. Planning on launching a project under $15k seems more likely to yield a successful campaign.

This dataset contains a few limitations, including:
1) There is only an average donation amount provided, a statistic that could be skewed by a large donation. For example, there were two successful projects with goal amounts of $50,000 or more and we don't know if one backer donated, for example, $49,900 and then all the other backers donated a few dollars each. 
2) This dataset does not provide information on the timeframe of each donation. We can provide better advice to those considering launching projects on the cruciality of getting backers in the beginning days/weeks of a campaign, vs. making a bigger push in the 2nd or 3rd weeks. 
3) This dataset does not state how long a project was spotlighted, or at what point it became a staff pick. Those timeframes could help further pinpoint when a project reached its goal. 

Finally, the graphs shown above are not the only ones we could create to analyze this dataset. We could also summarize data by:
- outcomes based on number of backers
- number of backers vs. goal amount and pledged amount
- country by country to determine if there are more desirable markets outside the US
