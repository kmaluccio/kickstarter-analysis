# An Analysis of Kickstarter Campaigns
## Overview
Perform an analysis on Kickstarter data to uncover trends and help Louise make decisions about her current Kickstarter.
We are interested in theater/plays in the US, so we focus on this parent/subcategory and country for our analysis.
More specifically, we analylze the data based on the launch date and goals chart from these similar kickstarters to deliver our results.
### Purpose
To help Louise learn about different kickstarter campaigns to compare with her campaign and help her be more successful.
## Analysis and Challenges
All data, descriptive and category statistics can be found in the excel file titled Kickstarter_Challenge saved in the repository.
For this analysis, we focused on the data in the category and subcategory theaters/plays. First, we looked at the launch date for all theater campaigns and summed up the total number of successful, failed, or canceled kickstarters based on the month of the launch. This information allowed us to calculate the launch month which has the most successful theater campaigns. This gives Louise an idea of when she might want to launch her campaign with the best chance of it being successful. Next, we want to compare the outcome of the kickstarter campaigns to their goal amount. To do this, we total the number of successful, failed, and canceled theater/play kickstarters based on five thousand increments of goal amounts from less than 1,000 to greater than 50,000. With this, we calculate the percentage of each outcome and graph the results to see which goal amounts are most successful in this category. When calculating this percentage, it is important to makae sure we are not dividing by zero. To avoid this error, we can write an if statement that checks the total projects being greater than 0 and if not, the result should be 0.

### Analysis of Outcomes Based on Launch Date
Here is the link to the bar graph of outcomes vs launch date for all kickstarters in the theater category: ![Theater_Outcomes_vs_Launch](https://github.com/kmaluccio/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
Here is the link to the line graph of outcome vs goal amount for each theater/play kickstarter: ![ParentCategoryOutcomes](https://github.com/kmaluccio/kickstarter-analysis/blob/main/ParentCategoryOutcomes.png)

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
The line chart for theater outcomes vs launch date, shows us that the most successful month to launch this kickstarter is in May and the least successful month is December. 
- What can you conclude about the Outcomes based on Goals?
We can conclude that the theater has the most number of successful campaigns which is good news for Louise and shows she has a better chance of being successful. However, Louise is asking for double the average goal amount for successful kickstarters which is not good for her campaign.
- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
