# Kickstarting with Excel
## Overview of Project
Louise started a kickstarter campaign for her play and wants to know how her campaign did in comparison to others. The data set includes various campaigns from different countries and categories. Sorting through the dense data to isolate the pertinent theatre data for Louise is the main goal. Through these actions, I hope to provide Louise with useful data-driven information.
### Purpose
Performing analysis on kickstarter campaigns to determine what benchmarks are vital in a successful campaign. Data from various categories and countries allow us to compare and contrast the different outcomes.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
I created a PivotTable from the Kickstarter sheet in order to produce a PivotChart visualizing campaign success by month. In order to produce this chart, I first created a new PivotTable in the sheet named Theatere Outcomes by Launch Date. I placed outcomes in both the Columns and Values fields; the Date Created Conversion was placed in the Rows field; and finally, the Filters field included Year and Parent Category. Once the chart was accurately depicting the data, I filtered the Parent Category to only show Theatre. 

![Theater_Outcomes_PivotTable](https://user-images.githubusercontent.com/102937467/163742780-fce0de99-0772-4512-a309-5fc04b475c91.png)

After the PivotTable was complete, I created a PivotChart. Per the module instructions, I created a line chart and named it Theatre Outcomes Based on Launch Date. 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/102937467/163743000-56564f3d-00b6-4270-95c3-bc4d1412aefc.png)

### Analysis of Outcomes Based on Goals
I created a chart and included the directed headers and goal ranges. Then I used the COUNTIFS function to filter out the desired data from the Kickstarter sheet. 

![Outcomes_Based_on_Goals_COUNTIFS](https://user-images.githubusercontent.com/102937467/163744438-1a6b4f36-8a7a-4e9b-809e-b4aec1e41bde.png)

The range for Less than 1000 was simpler than most of the cells. An additional criteria was added to accurately populate the desired range: 

![Outcomes_Based_on_Goals_COUNTIFS_2](https://user-images.githubusercontent.com/102937467/163744526-fc50e451-3838-42b8-9862-27f69da9b2b7.png)

Once columns B-D were populated, I utilized the SUM function in column E to populate the total amount of projects for each range. For columns F-H, I used the IFERROR function to calculate the percentage of each range/category: 

![Outcomes_Based_on_Goals_IFERROR](https://user-images.githubusercontent.com/102937467/163744686-090a1b6b-c729-4a22-8f24-5fa87427a373.png)

After filling out the chart, I created a line graph to depict the outcomes based on goal:

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/102937467/163744815-f0be01ad-ef8f-41c5-b9e2-075293ae6ad3.png)

### Challenges and Difficulties
I had quite a few challenges during this challenge, but working through them increased my excel knowledge. First, I'll explain the challenges within the Theatre Outcomes by Launch Date sheet. One of the first steps to this deliverable was to add a Year column in the Kickstarter sheet. I used the YEAR function, but it was populating an entire date rather than just the year. With the help of Wayland during office hours, we discovered I was using the wrong number format for the Year column. I changed the number format from Date to Number to resolve this. Next, I'll discuss the difficulties I had with the Outcomes Based on Goals sheet. The COUNTIFS function was simple for row 2, since there wasn't a range. The range gave me some difficulty, since it kept saying there was an error. I played around with it, but the error remained. Eventually, I applied the appropriate range for each cell. This solved the error problem. The next difficulty was with creating the graph. I understood what I needed to do, but excel was not allowing me to make the needed changes with the graph I selected. A friend of mine informed me of the various options of line graphs. Choosing the correct graph yielded my desired reults. The last difficulty I had was with the 50000 or More row. I accidently put an extra 0, and my graph was off. Once I fixed this, my graph matched the example in the module.
## Results
The two conclusions I can draw about the Theater Outcomes by Launch Date are (1) May is the best time to begin a kickstarter campaign, and (2) the trends between the failed and successful have a direct relationship.

My conclusions about the Outcome based on Goals are (1) the worst goal range is 45000 to 49999, while the best goal range is Less than 1000, and (2) the trends have an inverse relationsip.

Some limitations of the dataset, for our desired findings, are: year relevancy and diversity in outcomes. In regard to year relevancy, the most recent year in the data set is 2017. This poses as a problem, since there have been so many changes. One big change was the pandemic. As for the diversity in outcomes, there are no canceled campaigns. This may just be a coincidence, or it may be a lack of proper data collection for the canceled category. 

Another possible table which can be included in the data set is one analyzing the variables of the failed campaigns that fall within the most successful goal ranges. Through this analysis, we were able to reveal how vital the goal amount is. We can take this a step further in order to reveal what other benchmarks play a role in the outcome of a kickstarter campaign. 
