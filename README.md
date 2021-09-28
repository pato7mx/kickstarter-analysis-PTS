# Kickstarting with Excel

## Overview of Project

We are going to analyze a data set containing kickstarter campaigns, where we can see different data points such as: the goal and pledged amount $, the date the campaigned was launched, wheather the campaign reached its goal, among others.  
### Purpose

We want to use the data set to help our friend Louise understand how fundraising campaigns, specifically in the theather category, fared in relation to their launch dates and their funding goals. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

In the first part of the analysis, we observed the relationship between campaign launchdate vs outcome,successful, failed or canceled. This analysis was fairly simple as we only needed to add one single column to the data set, the column was named "Years" and it showed the year the different campaigns were launched. This was done by extracting the year from the "Date Created Conversion" column using the YEAR() formula. Finally, we created a pivot table and pivot chart in a new excel sheet where we could clearly visualize the data. Attached is an image of the pivot chart we created.


### Analysis of Outcomes Based on Goals

On the second part of the analysis, we observed the relationship between the goal amount vs the outcome. This analysis consisted on creating a table using the =COUNTIFS() excel formula where the columns were: Goal Range,	Number Successful,	Number Failed,	Number Canceled and	Total Projects. These columns were populated by filtering on different criteria using the =COUNTIFS() formula. For example the three outcome columns used the conditionals first to look for a goal range, which were on the goal column with different goals ranges in the rows, this were from less than a $1000 to greater than 50000 in $5000 increments. When the goal range was found the other crtiteria to populate the outcome columns were the outcome and the subcategory set to "plays". When the table was populated we created a line chart to visualize he relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y-axis. Chart Attached.


### Challenges and Difficulties Encountered

The main challenges encountered during the analysis were: 

I had a hard time using the COUNTIFS formula properly to populate the table for the analysis outcomes based on goals. I had some trouble as I wasn't very familiar with this formula and had some syntax errors when writing it, so I took a few tries until I got it right. I didn't encounter any other difficulties as I am fairly used to workig with data in excel and pivot tables and charts, but I can imagine someone newer to pivot charts might had had some trouble in the outcomes based on launchdate analysis.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

We can conclude that the best month to launch a campaign is may as it has the highest number of successful campaigns and also the highest percentage of success vs failure at 68%. Percaentage calculated dividing 111 successful campaigns by the sum of successful and failed campaigns at 163, so (111/163)*100 = 68%

We can also see that even though May has the highest number of successful campaigns it is not very different from other months when seen as a percentage of successful campaigns vs total campaigns as the average percentage of success vs failure looking at other months and excluding may is 62%

- What can you conclude about the Outcomes based on Goals?

We can conclude that for the most successful campaign rate the goal should be set to less than a $1000, as it is clear that as the goal amount increases the % of success decreases. Even though the line chart shoes a spike in success rate at the range of 35000 to 39999 it is not a great data point as it has a sample of only 6 projects and in general we can see a tendency for success rate to decrease as the goal amount increases. 

- What are some limitations of this dataset?

Of course it would always be better to have a larger data set to get to more reliable results so I would try to find a data set specifically on theather kickstarters to have more dat points to analyze.

- What are some other possible tables and/or graphs that we could create?

We could create a Box and Whiskers chart to analyze potential outliers in the data analyzed. 
