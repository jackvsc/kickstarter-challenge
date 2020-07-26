# kickstarter-challenge

## Overview of Project

We are assisting our client, Louise, in funding her new production, *Fever*, through kickstarter. We are exploring how different kickstarter campaigns fared in relation to their launch dates and their funding goals. These campaigns were created in 21 different countries between 2009 and 2017.

### Purpose

Our goal is to visualize the campaign outcomes in order to analyze how a campaign is effected by its launch date and its funding goal. This analysis will assist Louise in her current and future campaigns.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

Using a pivot table, the campaign data is first filtered to show only theatrical plays, as these campaigns are all we and Louise are interested in. Then a chart is created to show the amount of successful, failed, and canceled campaigns over their respective launch dates by calendar month.

![Outcomes Based on Launch Date](/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

A table is created in a new sheet to categorize the data by campaign goal amounts. The COUNTIFS function is used to call data from the original Kickstarter sheet. The data is filtered to show only plays, then filtered by campaign goal amount and the campaign outcomes, and placed in its proper category in the table. Then the count of successful, failed, and canceled campaigns is visualized in percentages for each campaign goal amount.

'=COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$D:$D,"<1000",Kickstarter!$R:$R,"plays")'

![Outcomes Based on Goals](/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

The **Theater Outcomes By Launch Date** chart is based upon the calendar month of launch dates for all years. A chart showing the outcome by launch date in each year leading up to 2017 may reveal a trend in campaign outcomes for each month, and could be valuable info for Louise's future campaigns.

The **Outcomes Based on Goal** chart shows the outcomes of campaigns by percentage. This may be misleading for campaigns with higher goals because only 15% of campaigns have a goal greater than $10,000.

Louise's current campaign for *Fever* came close to its funding goal in a short amount of time. A visualization of campaign outcomes based on campaign lengths may reveal valuable information for Louise's current and future campaigns.

## Results

- Theater campaigns almost always end with success rather than failure. Theater campaigns are most successful when commenced in May, and least so when commenced in December.

- Theater campaigns are most successful when the campaign goal is lower than $5,000.

- While the data set does contain the launch date and end date of each campaign, it does not contain the rate of funding for each campaign. For instance, Louise's campaign for *Fever* came close to its funding goal in a short amount of time. Understanding campaign outcomes based on the rate of funding for each campaign may reveal a pattern in campaign success and failure.

- A year-over-year visualization of campaign outcomes by launch date and a chart showing the number of campaigns for each goal category would each be valuable.
