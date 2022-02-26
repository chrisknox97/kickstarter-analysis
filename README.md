# Kickstarting with Excel

## Overview of Project 

### To uncover trends associated with successful Kickstarter-funded plays by means of launch date and fundraising goal. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

To conduct this analysis I first needed to transfer the "Date Created Conversion" column into a new column that would simplify the data into a single year using the YEAR() function. Once completed I created a Pivot Table using the raw Kickstarter data. I filtered the table by the newly created "Year" column as well as by "Parent Category", limiting results to theater. In addition, I eliminated any live campaigns from the data set as I was only interested in completed outcomes. 

For the Pivot Table, I placed "Outcomes" as my Column Field, "Date Created Conversion" as my rows, and "Count of Outcomes" as my values to fill in my table. From there I sorted the campaign outcomes in descending order for readability. Finally, I created a line chart from the curated data to visually depict "Theater Outcomes Based on Launch Date." The line chart may be accessed [here.](https://github.com/chrisknox97/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png) 

### Analysis of Outcomes Based on Goals

To conduct this analysis I needed to curate a new worksheet that would look at the success rates of plays based on Kickstarter goals needed for such success. For the columns I used Kickstarter Goal, Number of Successful, Failed, and Canceled Outcomes, Total Outcomes, and the Percentage of Successful, Failed, and Canceled Kickstarter projects. For the Kickstarter goals, I specified ranges starting at "Less Than 1000" that incrementally increased by 5000. 

I then used the COUNTIFS() Function specifying the following conditions: the specified goal range, whether I was looking for successful, failed, or canceled Kickstarters, and that I was only concerned with "plays" from the data's "Subcategory" column. Using the SUM() function, I combined the counts of each goal range's successful, failed, and canceled outcomes to get "Total Projects". From there, I simply divided successful, failed and canceled outcomes by the "Total Projects" to get the "Percentage Successful", "Percentage Failed", and "Percentage Canceled" respectively. These values were then used to create a line chart with the Goal Ranges as the X-axis, and the Percentages as the Y-axis to depict "Outcomes Based on Goals." The line chart may be accessed [here.](https://github.com/chrisknox97/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

The biggest challenges I faced completing this analysis were both human error that resulted in skewed and/or errored functions, and difficulty locating necessary tools needed to complete this assignment. The issue with incorrect inputs was resolved by automating repetitive tasks by double-clicking the bottom right corner of cells to eliminate unnecessary human error. The issue with locating necessary tools was solved simply by familiarizing myself with Excel's layout. 

## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?

Most Theater Kickstarter Campaigns are launched during the Summer months which correlates with the greatest success rates occurring in May (the peak), June, and July. As a result, the most advantageous period to launch this type of Kickstarter campaign would be in the Summer. 

Few Kickstarter campaigns for theater are canceled, with the highest total (7 in January) only amounting to seven percent of the total campaigns for that month. 

### What can you conclude about the Outcomes based on Goals?

Successful Kickstarter Campaigns for Plays are a mixed bag with one expecting such a campaign to succeed only half of the time. However, for the best chance at success, one should set a goal of $1000 or less (76% success rate). 

### What are some limitations of this dataset?

These datasets eliminate live or ongoing Kickstarter campaigns which could alter our results in the future. But more importantly, this data set features campaigns from 2014-2016, making them over a half decade old and potentially outdated for current analysis. 

### What are some other possible tables and/or graphs that we could create?

Another potentially useful charts would be a line graph that compares different countries' success rate based on Kickstarter goals or launch dates. We could also create a pie chart to visualize the percentage of successful theater productions in May (the most successful month). 
