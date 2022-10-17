# 1st Project for Ironhack Data Analytics Bootcamp

<img src="images/Other/Readme Photo.webp" width="1440" height="600">

### Description
This is a project that involves __cleaning and organizing data__. The project's goal is to analyze, clean, sort, and present the data in a way that demonstrates the validity or otherwise of a particular theory. The shark attack dataset was taken from Kaggle (the link can be found further down).

### Hypothesis 1: 
White sharks attack mainly men between 20 and 40 years old.


### Hypothesis 2: 
Fatality rate has decreased over the last 50 years in the USA.

### Process: 
Read the dataframe, make a copy and remove duplicates.

__H1:__

__Data Cleaning__ 
- Select variables and create a dataframe which we are going to use for evaluating the Hypothesis __(Age, Sex, Species).__
- Drop nulls and reset index.
- Make a list of the ages, create a new dataframe with the Updated Ages and concatenate it with the main dataframe for H1. Then convert the column to integer.
- Drop the age column as it will no longer be useful and set an order within columns.
- Make a list of white sharks, create a new dataframe with only white sharks, convert to string and capitalize. Then concatenate with main dataframe for H1.
- Drop species column.
- Localize and drop row in the Sex column that provides incorrect information.
- Sort per age for visual convenience.
- Export H1 cleaned dataframe to csv file.


__Data Visualization__
- Set predetermined configurations for graphs.
- __Graph 1__ - Display and plot attacks by sex and count victims.
- __Graph 2 & 3__ - Display attacks by age group and differentiate by victim's sex.
- __Graph 4__ - Boxplot to display the distribution and weight per age between sexes.

__Conclusion__

*Reflect on Hypothesis 1*
- __Men tend to be the sex most often attacked by white sharks, following a sort of normal distribution (as seen in Graphs 2 and 3), with most attacks occurring on men between 20 and 40 years of age. This result could be explained by the fact that this age and sex group is the most active and, therefore, the most likely to be attacked by white sharks.__

__H2:__

__Data Cleaning__
- Select variables and create a dataframe which we are going to use for evaluating the Hypothesis __(ID, Year, Date, Country, Fatal).__
- Drop nulls, take a look at the shape of the dataframe.
- Convert column 'Year' to integer.
- Check if there are duplicate ids, if there are, another record with the same ID(+x) is created. Apply the function to the H2 dataframe.
- Check content of column 'Country', to make sure we have suffcient data for 'USA'.
- Check number of IDs that ended in fatality and correct rows. Drop nulls.
- Check how many Years are unique (by comparing Year 0 and Date we see there is some information about the Year inside the date column, those intervals are going to be ignored).
- Check nulls.
- Set and apply the conditions needed to filter the dataframe H2.
- Drop 'Date' column and sort values by Year for visual convenience.
- Export H2 cleaned dataframe to csv file.

__Data Visualization__ 
- Dynamic table to see per year, the number of fatalities and the number of people that survived.
- We create two new columns, total (nº fatalities + nº of people that survived) and one for the % of fatalities respect to the total.
- __Graph 5__ - Evolution of Fatality rate in the USA.
- __Graph 6__ - Percentage of people that survive to attacks in the USA.
- __Graph 7__ - Number of people that died or survived due to attacks of sharks in the USA.

__Conclusion__

*Reflect on Hypothesis 2*
- __Fatality rate has decreased in the USA over the last 50 years as shown in Graph_5. We can see that the number of attacks have increased (Graph_7) but this may be due to lack of sufficient information from previous decades. The overall conclusion is that although attacks seem to have increased within the last decades, the % people that die due to these attacks, has been reduced.__

### Author:
Carlos Muñoz Fresco

### Documentation: 
The data comes from Kaggle (more specifically it is data that has been collected by the Global Shark Attack File) https://www.kaggle.com/datasets/teajay/global-shark-attacks

