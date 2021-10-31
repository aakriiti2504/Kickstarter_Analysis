# An Analysis of Kickstarter Campaigns with Excel
Performing analysis on Louise's Kickstarter data to uncover trends in various categories for organizing a number of events across different countries.

## Overview of Project
This project revolves around an upcoming playwright Louise who has started a crowdfunding campaign so that she can fund her play 'Fever'. The estimated budget for her play is over $10,000. Since this is Louise's first time dealing with a fund-raising campaign she is looking for some help with an in-depth analysis. 

#### Tools Used  
Throughout this project Microsoft Excel was used to sort, organize and analyze crowdfunding data. The detailed analysis will help in determining the specific factors that would help in making the campaign for Louise successful. Pivot tables and charts were used to visualize the data in a specific setup.

### Purpose
The purpose of this project is to analyze our data based on various parameters and draw conclusions based on the outcomes. The dataset provided mirrors a real world scenario that rquires data analysis and visualization. The main purpose of this project is to help Louise plan her crowdfunding campaign successfully so that she can meet her goals for the play 'Fever'. 

The detailed analysis would help Louise understand the trend and get an in depth insight into her campaign from start to finish. The findings will also help her to organize more such campaigns in the future and show her how she can determine factors important for a successful campaign. The analyzed data foucuses on helping Louise kickstart her production.

## Analysis and Challenges
Louise is planning to organize a crowdfunding campaign to fund her play 'Fever'. In a short duration, she came close to its fundraising goals. The kickstarter dataset was used to filter and organize data according to various needs and scenarios. 

### Challenges
There were a few challenges faced during the analysis. One of them being that the dataset was huge. The excel sheet consisted of 21 columns and 4115 rows of data. Filters were applied and cleared carefully. Before a new analysis or filter was applied, it was made sure that the old filters were cleared. when creating pivot tables, fields were carefully selected so that the desired tabular data could be generated. Chart title an dchart elements were also selected correspondingly. The COUNTIFS() function was complicated to use in the beginning and was carefully typed for each column. The 'live' outcome was deselected while filtering the pivot table for 'Outcomes vs Goals' in the 'plays' category.

### Analysis of Outcomes Based on Launch Date
The launch date in the dataset was given in the UNIX timestamp format hence it was required to convert the timestamp in readable format. A separate column 'Date Created Conversion' was created to convert the timestamp in the readable format. A pivot table was created using the 'Date created conversion' in the rows section. 'Outcomes' were put tn the columns and the values section whereas 'parent category' and 'years' was kept in th filter section. After the pivot table was created, the parent category was sorted for 'theater'. As a result all the count of outcomes were specific to the theater category.

![Theater_Outcomes vs launch table](https://user-images.githubusercontent.com/23488019/139595596-dc3d2706-c8a0-4f97-b38c-af03cb9bf286.png)

It can be noted that there are total of 839 successful, 493 failed and 37 canceled outcomes. The grand total of all these outcomes is 1369. The highest(111) and lowest(37) successful events were in the month of May and December respectively. The highest(52) and lowest(31)failed outcomes were in the month of May and November respectively. There were no canceled events in October and highest in January. January and March had same number of successful (56) events and failed (33) events. The month of May and June both have greater success rate. January, June, July and October had similar number of failed campaigns.


![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/23488019/139595573-4fa210e6-f7b7-4d67-b027-873f7047d765.png)



### Analysis of Outcomes Based on Goals
For outcomes based on goals, the goals were divided into 12 different categories from less than 1000 to greater than 50000. Number of successful, failed and canceled events were calculated by using the COUNTIFS() function. Filters used were the specific goal range, 'plays' subcategory and corresponding outcome for each row. It can be seen that there were '0' number of events 'canceled'. The total number of projects was calculated using the 'SUM()' function. Finally, the percentage of each outcome was calculated by dividing the number of certain outcome by the total number of projects. The 'Percentage' data format was used to display the result in percentage format. Since 'Number Canceled' was '0' for all rows, 'Percentage Canceled' was '0%' too.


![outcomes vs goals chart](https://user-images.githubusercontent.com/23488019/139595616-876574a3-64b2-4b13-b245-7a6be85f5c68.png)

From the chart it can be noted that the most number of successful (388) events were in the goal range of '1000 to 4999'. However the highest 'Percentage Successful' was 76% for 'Less than 1000'. The least (0) succesful  and 'Percentage successful' was in the range of '45000 to 49999'. The goal range of '15000 to 19999' had same values (12) for both 'Number Successful' and 'Number Failed'. The highest 'Percentage Failed' (100%) was for '45000 to 49999'. 'Greater than 50000' came a close second at 96%. '35000 to 39999' and '40000 to 44999' had same values for 'Percentage Successful' (67%) and 'Percentage Failed'(33%). They were also same for range '15000 to 19999' at 50%. The lowest 'Percentage Failed' was for 'Less than 1000' at 24%. 

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/23488019/139595518-98e3e33c-8016-4abf-bc4e-1f964804fc1b.png)
---

### Challenges and Difficulties Encountered

The challenges and difficulties encountered during the analysis of the kickstarter data is described below:

- A few challenges were encountered while working on the data. One of the major challenges faced was the huge data set. 

- Filters were applied and when new filters needed to be applied, care was taken to clear the previous filter to avoid errors and any discrepancies. One way to check that the filters were cleared was to check the serial number of the rows on the top. The ids in ascending order confirmed that all the entries were present and one could proceed with application of next set of filters.

- It was very important to carefully select the rows, columns, filters and values while creating the pivot table. A wrong selection of fields could completely change the results. 

- The COUNTIFS() function was carefully used to populate the "Number Successful", "Number Failed" and "Number Canceled"columns. The filters were carefully selected so that there is no confusion in populating these columns.

- The pivot table for 'Outcomes based on Launch Date' was carefully filtered for all 'theater' category and columns were sorted in the correct order of successful, failed and canceled. The 'live' column was omitted from the pivot table using the filter.

- While calculating the percentage in the 'Outcomes based on Goals' table, I spent a little time working on the decimals. I used the decrease decimal button and the percentage data type to get the desired format. In the formula used for calculating percentage, I was initially multiplying the result by 100 to get the percentage. However, realized that it was not needed when percentage data type was used and removed it from the formula for the respective columns.


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The two conclusions drawn from the 'Outcomes based on Launch Date' analysis are that the  month of May had the highest Successful outcomes as well as failed outcomes. There     were no canceled events in the month of October. The closest successful (37) and failed (35) outcomes were in the month of December. The month of May and June both have greater success rate. The month of May and June both have greater success rate. January, June, July and October had similar number of failed campaigns.
  
- What can you conclude about the Outcomes based on Goals?

For 'Outcomes based on Goals' it can be concluded that the 'Percentage Succesful' was highest (76%) for the goal range 'Less than 1000' and the highest 'Percentage Failed' was for the goal range '45000 to 49999'. There were no canceled events hence the Percentage canceled for all goal ranges were 0%.

- What are some limitations of this dataset?

Some limitations of the dataset are the fact that the dataset has UNIX timestamp and they had to be converted to readable date format. Because of the huge dataset, filters needed to be applied and cleared carefully. 

- What are some other possible tables and/or graphs that we could create?

 Since the dataset is huge, innumerable combinations of tables and charts can be generated from it. Some of the possibilities are shown below:



### - Edinburgh Research:

At the Edinburgh Festival Fringe, Louise was inspired by 5 plays that are shown in the tabular data. She wants to know how these plays were funded. Hence the Edinburgh Research was done. The Edinburgh Research shows the goal, pledged, average donation and number of backers for the specific 5 popular plays. This shows that specific data from the huge dataset can be found and retrieved to perform specific comparisons and calculations. The VLOOKUP() function was used to lookup the relevant data. She also wants to know if these plays were funded by Kickstarter.





![Edinburgh Research](https://user-images.githubusercontent.com/23488019/139599168-fbd726e6-ecb5-4c32-8ead-09a1ca381f81.png)


![Edinburgh research chart](https://user-images.githubusercontent.com/23488019/139599172-2df7e49b-1ea4-4eac-bfa9-c30ab09f9897.png)




---


### - Category Statistics:
 
 In this data table we can see how many theater category were successful, failed, canceled and live. It can be observed that the total number of successful theater events are 839. We can note that theater is a popular category and a successful campaign. The data around technology campaign shows that their trend lines are scattered all over the place. Hence they become less predictable.
 
 
![Category statistics table](https://user-images.githubusercontent.com/23488019/139599190-111dcd7f-6567-4cbb-976e-76214c4f73d8.png)


![Category Statistics](https://user-images.githubusercontent.com/23488019/139599191-68a7be8e-5928-4af8-aa64-ca2ed8b137ff.png)

 
 ---
 
 
 
### - All Outcomes Based on Launch Date for theater(Including Live):

This data is similar to what we created in the analysis exceptthe fact that we are showing the live outcomes in the table and chart too. The outcomes are based on the Launch Dates converted from the timestamps.


![All Outcomes based on launch date for theater table](https://user-images.githubusercontent.com/23488019/139599220-7056d5c2-961e-4fd7-bcfb-167d44dfd5a7.png)



![All Outcomes based on launch date for theater](https://user-images.githubusercontent.com/23488019/139599222-69101cbf-6d92-4829-b842-8ff5b33a5663.png)



---

### - Parent Category Outcomes:

This particular chart shows the successful, live, failed and canceled outcomes in the various parent categories all over the world. If needed the country can be filtered to one country or a combination of them.

        
 ![Parent category Outcomes chart](https://user-images.githubusercontent.com/23488019/139599249-dcda048a-831f-4adf-983d-277cb3cdf5a7.png)
 
  
 ---

 ### - Subcategory Statistics:
 
 From the tabular data it can be inferred that there were total 70 failed, 6 live and 238 successful plays in Great Britain. The chart according to the table is also displayed below.
        
        
        
 ![Subcategory statistics table](https://user-images.githubusercontent.com/23488019/139599260-1c03c257-8320-465f-9f8e-09cc6b5537d1.png)
 


 ![Subcategory statistics](https://user-images.githubusercontent.com/23488019/139599262-dc46e0ea-68e2-4f7c-947d-d66a45a22d90.png)
 
 
 ---
 
 
 
 ### - Descriptive Statistics:
 
 The dataset can be used to calculate the mean and other statistical values. The tabulated datat can be seen in the picture below. Various statistical formulas can be used to calculate the same. Here, the mean, median, upper and lower quartiles, inter quartile ranges for goal and pledged columns have been calculated. With the inclusion of statistical data, Louise can carry on with her campaign with confidence. Information is presented to Louise so that she can be informed of the campaign strategy. The organization and sorting of data provides strength to our analysis.
 
![1 5 2 table](https://user-images.githubusercontent.com/23488019/139599785-38a71e09-2168-46ef-a2c2-2cdd90876315.png)
---
