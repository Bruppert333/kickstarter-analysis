# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of the analysis "Theater outcomes based on Launch date" was to see which months are the best to start a funding campaign. The purpose of the "Outcomes Based on Goals" was to see the percentage of successful, failed, and canceled campaigns based on how much their goal was.
## Analysis and Challenges
 
### Analysis of Outcomes Based on Launch Date
I performed the "Theater outcomes based on Launch date" by first creating another column in the kickstarter sheet named "years" ![Years_Screen_Shot](Documents/DataAnalytics/Module 1/Module 1 Challange/Show Work/Years_Screen_Shot.png). I used the formula =Year(Date Created Conversion) to get year each campaign started. I then selected all the data in the kickstarter sheet and created a Pivot table that filtered outcomes and years, and showed the amount of successful, failed, and canceled theater campaigns based on the month. ![Pivot_Table](Documents/DataAnalytics/Module 1/Module 1 Challange/Show Work/Pivot_Table.png) ![Table_Filter](Documents/DataAnalytics/Module 1/Module 1 Challange/Show Work/Table_Filter.png)
### Analysis of Outcomes Based on Goals
I performed the "Outcomes Based on Goals" by using the =COUNTIFS() formula. Each formula had to be typed in manually to get the Goal Range correct. ![Count_Ifs_Example](Documents/DataAnalytics/Module 1/Module 1 Challange/Show Work/Count_Ifs_Example.png). I then used the Sum formula to break down each successful and failed campaigns based on thier goal range. ![Sum_Example](Documents/DataAnalytics/Module 1/Module 1 Challange/Show Work/Sum_Example.png). After I got the total of failed and successful campaigns based on goal amount. I was able to get the percentage by dividing either the number of successful or failed campaigns by the total project. ![Percent_Example](Documents/DataAnalytics/Module 1/Module 1 Challange/Show Work/Percent_Example.png).
### Challenges and Difficulties Encountered
The challange of the "Theater outcomes based on Launch Date" was figuring out which fields to use in the pivot table. I think the best way to figure this out is by moving things around until it portreys the data how you want it to be. The challenge I faced with "Outcomes Based on Goals" was with the =COUNTIFS() formula. The formula wasn't recognizing the "Less than" and the "to" between the number ranges. I overcame this by using the formula =COUNTIFS(Kickstarter!F:F,"successful",Kickstarter!R:R,"plays", Kickstarter!D:D,">=5000",Kickstarter!D:D,"<=9999") to sort the data by the amount of successfull plays that goals were between $5,000 to $9,000.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    One conclusion I can draw about the "Theater Outcomes based on Launch Date" is that the best time to Launch a successful Theater Campaign is in the summer. Specifically May and June. Another conclusion about this analysis is that there isn't really a difference in canceled campaigns month to month, most people will continue their campaign rather it fails or succeeds.
- What can you conclude about the Outcomes based on Goals?
    I can conclude that although not a lot of campaigns were asking for super large amount of money, the ones that did had a higher fail rate. If the play's goal was under $5,000, they had a higher success rate. 
- What are some limitations of this dataset?
    I guess I'm not sure what limitations of this dataset would be. As I was looking through the data and thinking what other types of things I would like to know would be states or cities. For example, it may be helpful to know not only the country, but what region or state they took place. This would give a better analysis to show if some states were more likely to donate than others. 
- What are some other possible tables and/or graphs that we could create?
    I think a graph that looks good for this type of data is a stacked bar graph. For example, the "Outcomes Based on Goals", it is easy to read the data if the successful and failed is stacked on top of eachother out of 100% to visually see if more or less failed or succeeded. ![Alternative_Chart](Documents/DataAnalytics/Module 1/Module 1 Challange/Show Work/Alternative_Chart.png).  