# Kickstarting with Excel

## Overview of Project

### Purpose
- Louise's play Fever came close to its fundraising goal in a short amount of time. Now, she wants to know how different campaigns fared in relation to their launch dates and their funding goals. 
- Using the Kickstarter dataset, I visualize campaign outcomes based on their launch dates and their funding goals, and provide this written report based on my analysis and the visualizations created here.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
![Outcomes Based on Launch Date](resources/Theater_Outcomes_vs_Launch.png)
- We can see that the months of May and June both have a greater success rate.
- The months of May, Jun, Jul, Aug and Oct have similarly high number of failure rate.
- The canceled rate in January is the highest.
- Here is the link to [Kickstarter_Challenge.xlsx](Kickstarter_Challenge.xlsx).

### Analysis of Outcomes Based on Goals
![Outcomes Based on Goals](resources/Outcomes_vs_Goals.png)
- We can see the higher percentage of success for Goals in less than 1k, 1k-1.5k, 35k-40k, and 40k-45k (75.81%, 72.66%, 66.67%, 66.67%).  
- Higher percentage of failed for the Goals in 25k-30k, 45k-50k =, and over 50K (80%, 72.73%, 100%, 87.5%). 
- Here is the link to [Kickstarter_Challenge.xlsx](Kickstarter_Challenge.xlsx).

### Challenges and Difficulties Encountered
- One challenge is to setup `COUNTIFS` formulas in the sheet "Outcomes Based on Goals". By copy and paste the formulas to other columns without using absolute cell reference will require lots of updates in the formula. By adding absolute cell reference, it makes my life easier!
``` 
=COUNTIFS(Kickstarter!D:D,">=5000",Kickstarter!D:D,"<=9999",Kickstarter!F:F,"successful",Kickstarter!R:R,"plays")
=COUNTIFS(Kickstarter!$D:$D,">=5000",Kickstarter!$D:$D,"<=9999",Kickstarter!$F:$F,"successful",Kickstarter!$R:$R,"plays")
```
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The month that launched the most successful Kickstarter campaigns was May.
However, May, June, July, August and October all had roughly the same number of failed campaigns launched.

- What can you conclude about the Outcomes based on Goals?

It is more likely to have successful outcome if the Goal is less than $1000, or between $1000 to $1500.

- What are some limitations of this dataset?

The latest data was drawn from 2017, which is a little outdated. It is suggested to extract some recent data from the internet, in order to make the results more updated.

- What are some other possible tables and/or graphs that we could create?

We may further filtering the graphs with the Country like GB or US, depending on where Louise is planning to perform the play, to make the results more specific and realistic. 
