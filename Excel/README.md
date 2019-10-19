# Unit 1 Homework: Kickstart My Chart

## Assignment

Over $2 billion has been raised using the massively successful crowdfunding service, Kickstarter, but not every project has found success. Of the more than 300,000 projects launched on Kickstarter, only a third have made it through the funding process with a positive outcome.

Getting funded on Kickstarter requires meeting or exceeding the project's initial goal, so many organizations spend months looking through past projects in an attempt to discover some trick for finding success. For this week's homework, you will organize and analyze a database of 4,000 past projects in order to uncover any hidden trends.

## Instructions

![Kickstarter Table](Images/FullTable.PNG)

Using the Excel table provided, modified and analyze the data of 4,000 past Kickstarter projects to uncover some market trends.

* Used conditional formatting to fill each cell in the `state` column with a different color, depending on whether the associated campaign was successful, failed, or canceled, or is currently live.

  * Created a new column O called `Percent Funded` that uses a formula to uncover how much money a campaign made to reach its initial goal.

* Using conditional formatting to fill each cell in the `Percent Funded` column using a three-color scale. 
  * Created a new column P called `Average Donation` that uses a formula to uncover how much each backer for the project paid on average.


  * Created two new columns, one called `Category` at Q and another called `Sub-Category` at R, to split the `Category and Sub-Category` column into two parts.

  ![Category Stats](Images/CategoryStats.PNG)

  * Created a new sheet with a pivot table that analyze initial worksheet to count how many campaigns were successful, failed, canceled, or are currently live per **category**.

  * Created a stacked column pivot chart that can be filtered by country.

  ![Subcategory Stats](Images/SubcategoryStats.PNG)

  * Created a new sheet with a pivot table that analyze initial sheet to count how many campaigns were successful, failed, or canceled, or are currently live per **sub-category**.

  * Created a stacked column pivot chart that can be filtered by country and parent-category.

* The dates stored within the `deadline` and `launched_at` columns use Unix timestamps. Fortunately for us, [there is a formula](http://spreadsheetpage.com/index.php/tip/converting_unix_timestamps/) that can be used to convert these timestamps to a normal date.

  * Created a new column named `Date Created Conversion` that will use [this formula](http://spreadsheetpage.com/index.php/tip/converting_unix_timestamps/) to convert the data contained within `launched_at` into Excel's date format.

  * Created a new column named `Date Ended Conversion` that will use [this formula](http://spreadsheetpage.com/index.php/tip/converting_unix_timestamps/) to convert the data contained within `deadline` into Excel's date format.

  ![Outcomes Based on Launch Date](Images/LaunchDateOutcomes.PNG)

  * Created a new sheet with a pivot table with a column of `state`, rows of `Date Created Conversion`, values based on the count of `state`, and filters based on `parent category` and `Years`.

  * Then created a pivot chart line graph that visualizes this new table.

# Created a report in microsoft word and answered following questions.

1. Given the provided data, what are three conclusions we can draw about Kickstarter campaigns?

Following are the three conclusions after looking at the Kickstarter campaigns data:

1.	Theatre, Music and Film & Video are the most successful category of campaigns, resulting in a 15% higher total revenue generation than the initial total goal for these three categories.

2.	Following the trends of the parent category, plays, rock and documentary are the most successful campaigns. Hardware has 0 failed or canceled campaigns and is one of the most fruitful campaigns with all successful campaigns so far. 

3.	Considering all years since 2009, February, May, October are the most successful months in terms of new launches. The months of March and September have a steep drop in terms of successful campaigns. September also shows a decrease in failure campaigns.  June and July months show an increase in failure and canceled campaign respectively.
 

2. What are some limitations of this dataset?

We have a good chunk of data to analyze some of the major trends. I think we cannot understand why some campaigns in the same sub-categories are doing great and why some are not at the moment. It can be achieved if we do further scrutiny of the data to create and analyze more trends or if we can identify reasons for success/failure/cancel of any campaign.

3. What are some other possible tables and/or graphs that we could create?

Ans:
1.	We could also look at some tables or graphs to see the trends between all the sub-categories for an individual parent category to evaluate the behavior.
2.	We could maintain individual line charts for live projects of the respective sub-categories to keep a track for upcoming months.
3.	We could calculate success rate, profit or Loss and create charts with respect to parent categories or sub-categories.
4.	We could create charts to analyze categories and sub-categories’ Vs Month/Year charts.


## Bonus

* Created a new sheet with 8 columns:

  * `Goal`
  * `Number Successful`
  * `Number Failed`
  * `Number Canceled`
  * `Total Projects`
  * `Percentage Successful`
  * `Percentage Failed`
  * `Percentage Canceled`

* In the `Goal` column, created 12 rows with the following headers:

  * Less than 1000
  * 1000 to 4999
  * 5000 to 9999
  * 10000 to 14999
  * 15000 to 19999
  * 20000 to 24999
  * 25000 to 29999
  * 30000 to 34999
  * 35000 to 39999
  * 40000 to 44999
  * 45000 to 49999
  * Greater than or equal to 50000

  ![Goal Outcomes](Images/GoalOutcomes.PNG)

* Using the `COUNTIFS()` formula, count how many successful, failed, and canceled projects were created with goals within the ranges listed above. Populated the `Number Successful`, `Number Failed`, and `Number Canceled` columns with this data.

* Add up each of the values in the `Number Successful`, `Number Failed`, and `Number Canceled` columns to populate the `Total Projects` column. Then, using a mathematical formula, find the percentage of projects that were successful, failed, or canceled per goal range.

* Create a line chart that graphs the relationship between a goal's amount and its chances at success, failure, or cancellation.

## Submission

* Updated Excel Homework submitted https://github.com/poonamsumedh2/BCampassign

- - -

© 2019 Trilogy Education Services
