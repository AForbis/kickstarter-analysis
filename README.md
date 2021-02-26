__Kickstarting with Excel__

__Overview of Project__

Following Louise's funding campaign for her play Fever, she wanted to better understand the relationship, if any, between a campaign's launch date and a campaign's funding goals. To help Louise understand these relationships I combed through the Kickstarter dataset and created two charts to visualize how a campaign's launch date and funding goals might affect its outcomes.

__Analysis and Challenges__

Analysis of Outcomes Based on Launch Date

- To prepare for this visualization, I first created a new "Years" column in the dataset that would extract the year from the existing "Date Created Conversion" column. This  would make sorting and analyzing the data easier within a pivot table and would produce a cleaner and more effective x-axis for the visualization. With the data ready, I then created the pivot table, being sure to break out the campaign outcomes by month for easier viewing. I added a years filter in case Louise wanted to see how campaign's fared year to year, but left the filter untouched so she could see the aggregated outcomes from all years with data (2010-2017). To make the visualization more applicable to Louise's campaign, I filtered out all the parent categories except for theater. With the pivot table ready, I chose to create a line chart because of its ability to effectively visualize data trends over time. In the chart below, Louise can see the total number of successful, failed, and canceled theater campaigns from 2010-2017.

![](Theater_Outcomes_vs_Launch.png)

[Review the "Theater Outcomes by Launch Date" tab for a closer look at the data](Kickstarter_Challenge.xlsx)

__Analysis of Outcomes Based on Goals__

- To prepare for this visualization, I created a new sheet with a table that broke down fundraising goal amounts into 12 separate buckets (e.g., less than 1000, 1000-4999). Using the countifs() function, I calculated the number of successful, failed, and canceled plays for each fundraising goal range. Afterwards, I created a column that totaled the number of successful, failed, and canceled plays. With this column in place, I then proceeded to divide each the number of successful, failed, and canceled plays by the total number of plays in order to calculate the percentage of the whole for each outcome. With the data ready, I proceeded to make the line chart below that plotted the percentage of successful, failed, and canceled plays across each fundraising goal range.

![](Outcomes_vs_Goals.png)

[Review the "Outcomes Based on Goals" tab for a closer look at the data](Kickstarter_Challenge.xlsx)

__Challenges and Difficulties Encountered__

The biggest difficulty I encountered was after I completed the modules and was beginning the challenge when Excel crashed and I lost several of the pivot tables I had created. It was a much needed reminder for me to save early and often! Another difficulty I encountered was making sure I used the proper mathematical symbols when nesting formulas within countifs() function. I caught a few errors when proofreading the first column. This was a good reminder of how tedious I expect future coding assignments to be and how I will need to keep a watchful eye for errors and have effective debugging protocols in place to reduce the probability of errors.

__Results__

Outcomes based on Launch Date

1) From 2010-2017, the month of May had the highest number of successful theater campaign fundraisers. This suggests that the month of May is the best month to launch a theater campaign.

2) From 2010-2017, the number of successful theater campaign fundraisers peaked in May and decreased each subsequent month for the rest of the year (except in October). This suggests that the chance your theater campaign fundraiser is a success decreases each month after the month of May.

3) From 2010-2017, the number of failed theater campaigns never surpassed the number of successful theater campaigns, but came the closest in December. This suggests that the chance of launching a successful theater campaign is higher than launching a failed one all year round.

Outcomes based on Goals

1) From 2010-2017, plays with a fundraising goal under $1,000 had the highest percentage of success. This suggests that launching a fundraiser for a play under $1,000 is the most likely to succeed.

2) From 2010-2017, the linear trendlines for both the percentage of successful and failed campaigns would suggest that a campaign's chances to reach their goal typically decreases the higher the fundraising goal amount is set at.

__Limitations__

One limitation is that approximately 85% of the play campaign fundraisers had goals under $10,000, which makes drawing conclusions about the outcomes of play fundraisers with higher goal amounts more difficult because there a far fewer to analyze and thus could be more influenced by outliers. Additionally, approximately 75% of all campaign fundraisers were based in the U.S., which makes drawing conclusions about non-U.S. countries more difficult due to their underrepresentation in the dataset. To alleviate these concerns, future projects could collect more data from fundraisers over $10,000 and from more fundraisers outside of the U.S.

__Recommendations for additional graphs/tables__

Future graphs/tables of interest might include: (a) Theater Campaign Outcomes by Country, (b)Average Donations for Theater Campaigns by Country, and (c) Theater Campaign Outcome by Number of Backers.
