# An Analysis of Kickstarter Campaigns
## Overview
Perform an analysis on Kickstarter data to uncover trends and help Louise make decisions about her current Kickstarter.
We are interested in theater/plays in the US, so we focus on this parent/subcategory and country for our analysis.
More specifically, we analylze the data based on the launch date and goals chart from these similar kickstarters to deliver our results.
### Purpose
To help Louise learn about different kickstarter campaigns to compare with her campaign and help her be more successful.
## Analysis and Challenges
All data, descriptive and category statistics can be found in the excel file: [Kickstarter_Challenge](https://github.com/kmaluccio/kickstarter-analysis/blob/main/Kickstarter_Challenge.xlsx).

For this analysis, we focused on the data in the category and subcategory theaters/plays. First, we looked at the launch date for all theater campaigns and summed up the total number of successful, failed, or canceled kickstarters based on the month of the launch. This information allowed us to calculate the launch month which has the most successful theater campaigns. This gives Louise an idea of when she might want to launch her campaign with the best chance of it being successful. Next, we want to compare the outcome of the kickstarter campaigns to their goal amount. To do this, we total the number of successful, failed, and canceled theater/play kickstarters based on five thousand increments of goal amounts from less than 1,000 to greater than 50,000. With this, we calculate the percentage of each outcome and graph the results to see which goal amounts are most successful in this category. When calculating this percentage, it is important to make sure we are not dividing by zero. To avoid this error, we can write an if statement (using the function IFERROR()) that checks for an error and if the result we want gives an error, then the result should be 0. Another challenge that can present itself is if there are any outliers in the data. We can use averages or temporarily ignore the outlier data to get results that make more sense as long as we remember to consider the outlier(s). 

### Analysis of Outcomes Based on Launch Date
This is the bar graph of outcomes vs launch date for all kickstarters in the theater category: ![Theater_Outcomes_vs_Launch](https://github.com/kmaluccio/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
This is the line graph of outcome vs goal amount for each theater/play kickstarter: ![Outcomes_vs_Goals](https://github.com/kmaluccio/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
One challenge encountered with the data was for the deadline and launch dates. These dates were in Unix timestamps, so they had to be converted to find out the actual day/month/year of the launch or deadline. There is a formula that we can use along with the DATE() function in excel to convert the timestamps appropriately.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
The line chart, for theater outcomes vs launch date, shows us the most successful month to launch this kickstarter is in May and the least successful month is December. So, this can help Louise determine when she it is in her best interest to launch her campaign.
- What can you conclude about the Outcomes based on Goals?
Kickstarters were more successful when the goal amount was $5000 or less and again rather successful between $35000 - $45000. Louise is asking for double the average goal amount for successful kickstarters which is not good for her campaign.
- What are some limitations of this dataset?
Limitations to the dataset include not being able to rate interest in the specific name/blurb of the kickstarter. Meaning, there may be some plays that an audience is more interested in so this would be more successful regardless of the goal amount or launch date. Since Louise is only considering these two variables, she might be missing other factors to compare her success to others.
- What are some other possible tables and/or graphs that we could create?
We can graph the parent category vs outcomes to see which category is most successful. From this, we conclude that the theater has the most number of successful campaigns which is good news for Louise and shows she has a better chance of being successful based on the category she chose. However, this does not mean she will definitely be successful, so this is not the most helpful result of the analysis. Also, we could create a comparison of both goals and launch date vs outcome in countries other than the US, if Louise was interested in starting a kickstarter in another country. We could have made more tables or graphs with the pledged data, but we found that the percentage of funding for each successful kickstarter was mostly over 100% and it was what you would expect for those that failed or were canceled (funding close to 0%). Thus, this information is not helpful to Louise.
