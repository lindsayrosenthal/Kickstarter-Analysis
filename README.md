# Kickstarter-Analysis
Outcomes based on analysis of Kickstarter Data
##The Purpose of this Analysis:
The client wants to know how different campaigns fared in relation to their launch dates and their funding goals. By creating visuals of the campaign outcomes, we can analyze how they performed.
##Analysis and Challenges
Using an excel function and pivot table I created visuals to show the client the relationship between the launch date and the success of the theater campaign. These visuals will allow us to make an analysis of the trends we see.

####**Analysis** - Theater Outcomes based on Launch Date 
1.Used the Year function to pull the year from the Launch Date column
  -`=YEAR()` 
  >Returns the year corresponding to a date. The year is returned as an integer in the range 1900-9999 from cell specified.
2.Created a Pivot Table based on Kickstarter Data with the following:
  -Filters:
    -Category,Years
  -Rows:
    -Date Created Conversion
  -Columns:
    -Outcomes
  -Values:
    -Count of Outcomes
 <font_color="grey">[Pivot Table Help]</font>[https://support.microsoft.com/en-us/office/create-a-pivottable-to-analyze-worksheet-data-a9a84538-bfe9-40a9-a8e9-f99134456576]
 3.Cleaned and Filtered the Data
  -Filtered:
    -Category based on Parent Category **Theater**
    -Column Labels to show successful, failed, and cancelled in descending order.
 4.Created a Line Chart to Visualize the findings.
 **PUT A URL TO THE LINE CHART IN RESOURCES**
 
#### **Analysis** - Theater Outcomes based on Goals 
Using excel functions I created a visual to show the client how many campaigns succeeded, failed, or were cancelled based on, if they were in a dollar certain range for their goal. This one required more excel function usage to calculate the values. 
Column references are from File: **ADD FILE FOR EXCEL FROM REP**
1.Calculations:
  -Columns B:D
    -`=COUNTIFS()`
    - =COUNTIFS('REF SHEET'!$D:$D,">=RANGE",'REF SHEET'!$D:$D,"<=RANGE",'REF SHEET'!$F:$F,"OUTCOME")
  <font_color="grey">[COUNTIF Function Help]</font>[https://support.microsoft.com/en-us/office/countif-function-e0de10c6-f885-4e71-abb4-1f464816df34]
  -Column D
    -`=SUM()`
    -=SUM(B:D) **B+C+D**
  <font_color="grey">[Sum Function Help]</font>[https://support.microsoft.com/en-us/office/sum-function-043e1c7d-7726-4e80-8f32-07b23e057f89]
  -Columns F:G
    - % Success=ColumnB/ColumnE
    - % Failed =ColumnC/ColumnE
    - % Canceled =ColumnD/ColumnE
    Set these columns format to percentage with no decimals.
 2.Created Line Chart Visual
    - Selected columns A(Goal) and F,G,H (Percentage Outcomes)
	  - Created line chart to display Outcomes Based on Goals
 **PUT A URL TO LINE CHART IN RESOURCES**
 #### **Challenges**
 I had some issues thinking I could copy the code from columns B:D but I realized the countif was very particular to column A. I also did not know how to put in a range such as 2-4 vs just >2.
 **Solution**: I watched a video on Countif and learned that I had to manually plug in more data for columns B:D and that the range issue would be solves by adding 2 different criteria. 


 
 


### Analysis of Outcomes Based on Launch Date

### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
