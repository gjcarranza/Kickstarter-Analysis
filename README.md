# Kickstarter-Analysis
Overview of Project: 

The purpose of this analysis is to provide insight of pre-dominantly past kickstarter campaigns success and fail rates, and provide insight of the possibility of success with the client's kickstarter campaign for their theater play.

Analysis and Challenges: 

The analysis is conducted via various treatments on excel. Two of which promotes stronger evidence and gives better insight on possible tactics to utilize and ensure a successful campaign. The image shown below is produced by using the pivot table feature and organizing the correct values to be implemented within its corresponded elements. The challenge of this portion of analysis is figuring out which filters go where. By reviewing previous exercises from past work, one quickly realized the filter that was missing to produce the correct information to display.

![image](https://user-images.githubusercontent.com/92961267/138585166-6f1cbe67-326a-4124-bbb1-0567b6b866d6.png)

Prior to visualing the image below, a table was created to encode such information.

=COUNTIFS('Raw Data'!$D:$D,">=1000",'Raw Data'!$R:$R,"r/plays",'Raw Data'!$F:$F,"successful")

This code was used for goals less than $1000 and for greater than $50,000. A secondary code which required more criteria:

=COUNTIFS('Raw Data'!$D:$D,">=1000",'Raw Data'!$R:$R,"r/plays",'Raw Data'!$F:$F,"successful",'Raw Data'!$D:$D,"<=4999") 

was used for goals that had a range. In order to get the percentage of successful, failed, and canceled outcomes, a ratio must be calculated prior to graphing. An example of such coding is provided below.

=SUM(B2:D2)

This is used to calculate the total number of projects for each row. An absolute total was calculated in the 'Total Projects' column of which was utilized in calculating the percentages for successful, failed, and canceled kickstarter campaigns (coding provided below)

=((B2/E14)*100)
	
![image](https://user-images.githubusercontent.com/92961267/138612751-521f1e91-f09a-49d4-a597-590f0d0f9647.png)

The following image displays the percentage of each respected row within the following three columns: 'Percentage Successful', and 'Percentage Failed'. The Percentage Canceled' is excluded as there are no canceled theater plays. 

![image](https://user-images.githubusercontent.com/92961267/138613144-9d843c28-07a8-4a1b-a723-4882ffa08bc7.png)

The challenge of this portion was not so much of a challenge but rather a moment of tediously repeating and editing the code to execute the correct calculation. There were issues on a personal end of which the code was implemented incorrectly, had missing criteria, or automatic selection of the wrong cell.

Results:

In conclusion, the client may have a higher success rate in meeting their campaign goal if the launch date were closer to a seasonal period (i.e. preferably between the months of April and July, more specifically June) as these dates may perhaps have better timing and donors may have more leeway with donations. A further analysis in donor's month-to-month finances and how much they have leftover for free-spending in addition to conducting and analyzing a survey as to the reason of the rise and decline of donations (e.g. saving money for holidays, other expenses, etc.) may be required to provide a more solid conclusion as to the reason why within this period campaigns tend to meet their goal. As for the graph "Outcome based on Goals", the client may be more inclined to reduce their goal or set their goal in increments over a longer-than-normal time span as the average time span for a campaign seems to be only a month. The recommendation to the client is to start their campaign some time in April and end in early July. However the limitations of the data set is not being able to view the average donations versus launch date period within the respective criteria of successful, failed, or canceled theater plays.
