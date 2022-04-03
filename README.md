# Kickstarter Analysis
## Kickstarting with Excel
Module 1 Analysis by Lauren Debes
## Overview of Project
Louise, a playwright, wants help researching crowdfunding to make her play "Fever" as successful as possible. We will be using Excel to analyze, sort, and organize data from a crowdfunding site.
## Purpose
We want to determine whether there there are specific factors that make a project's campaign successful. We will look at how timing and goal amount impacts success. She is estimating a budget of over $10,000, we will see if that is a reasonable goal.
## Analysis and Challenges
We will take a look at if launch date, based on month, of a kickstarter for plays has any effect on the success of a play. Then we will look at the correlation between goal and success of a campaign. 
## Analysis of Outcomes Based on Launch Date
We made a pivot chart from the data filtering to show only theater as the parent category. We also added the option to filter by year if Louise chooses, to see if theres been any changes in trends. Our rows consist of the month the campaign started, so there is one for each month. The columns are separated by successful, failed, cancelled, and the grand total number of campaigns. We then created a line graph to represent the findings. We used a line graph because it would clearly show the change by month and allowed us to see successful/failed/cancelled all at the same time.

Our findings showed that campaigns were most successful when started in May. The other summer months, June and July, were the next highest. May and October had the greatest number of failed campaigns. Cancelled campaigns generally remained the same month by month.

![Theater_Outcomes_vs_Launch.png](https://raw.githubusercontent.com/LaurenDebes/KickstarterAnalysis/main/Theater_Outcomes_vs_Launch.png)

## Analysis of Outcomes Based on Goals
We then wanted to analyze how often a campaign was successful based on the amount of the goal. The amounts were separated into $5,000 increments. We used the COUNTIFS function to count the number of successful, failed, and canceled campaigns within each goal. We then broke it into percentages to create a line graph from; using percentages gave a better picture of the data. We found that percentage successful generally went down the greater the outcome goal, except for a bump between $35,000-45,000. The percentage failed generally increased the greater the outcome goal, except for again between $35,000-45,000. There were zero cancelled plays. We used a line graph to clearly show up the changing percentages by category.
![OutcomesAndGoals](https://raw.githubusercontent.com/LaurenDebes/KickstarterAnalysis/main/Outcomes_vs_Goals.png)

## Challenges and Difficulties Encountered
Our "outcomes based on launch date" graph could perhaps be more informative if we used *percentage* of successful/failed/canceled campaigns for each month rather than the overall count. It looks as though the highest month for failed campaigns was in May, the same month where there was the highest number of successful campaigns, but if we used percentage we would know it only looks this way because there is the largest grand total of campaigns started in May. I would argue we do not need to analyze cancelled campaigns and they do not have a great impact on our data. We should also filter by country.

A potential challenge would be forgetting to filter out the "outcomes based on goals" to only look at "plays." It was also very important to include $ symbols before all of the columns that stayed the same, so that you could quickly drag the formula between columns. At first I did not realize the $ needed to be added and all of the formulas moved over incorrectly and would have taken awhile to correct. Luckily I caught it though! There were zero plays canceled, I dont think its worth keeping that category.
## Results
Our results showed that for "Outcomes based on Launch Date" the summer months generally had a greater rate of successful campaigns than the winter months. The successful versus failed line graphs follow a somewhat similar pattern, likely due to the grand total shifting. We can conclude that Louise should start her campaign during the summer and avoid campaigns in the Fall/Winter. The results also show that more campaigns are successful than failed.

Our results showed that for "outcomes based on goals" there were more successful campaigns for lower goals than higher goals. There was a range between $35,000-$45,000 where the inverse became true. More analysis on why this occured would be helpful. The most campaigns were successful when the goal was between $5,000-9,999. Louise should lower her $10,000 goal.

Some limitations of this dataset include not separating independent producers from well-established theaters. Some individuals wanted to fund a play are starting from scratch, while others have communities that have supported and donated to kickstarters in the past and have a wider audience already. 

Some other possible tables/graphs are another line graph for Theater outcomes by launch date, but by percentage rather than cumulative total. A 100% stacked bar graph could also be made and separated by month, but that would be harder to read. A bar graph could be used for outcomes based on goal instead, that would look similar. I think it would also be informative to make a line graph comparing average pledge and the success of a campaign. A graph looking at how long a campaign lasted versus success/fail would also be helpful.
