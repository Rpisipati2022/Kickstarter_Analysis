# Kickstarter_Analysis
Analysis of Kickstarter campaigns for plays
# Project Background
Background: a detailed analysis of Kickstarter campaigns to fund plays was conducted to provide Louise with viable fund raising goals for her play – these included the total amount she would ask for as well as timing for the campaign. Having successfully conducted a campaign, she wanted to know how other campaigns performed – vs. their funding goals and campaign timing. 

Purpose of current analysis: To better understand how different fundraising campaigns for plays fared both in relation to their launch dates (does it depend on when during the year a campaign is launched?) and original fund-raising goal (does the total amount impact success of the campaign?)

## Analyses
1. Outcomes vs Launch Date:
Created a pivot table by launch date, filtering on main category (Theater) and Year. Discarded the Quarter and Year that the date conversion automatically displayed and was left with month as rows. This showed all three selected outcomes (successful, failed, canceled) by month of launch.

[Outcomes by Month.pdf](https://github.com/Rpisipati2022/Kickstarter_Analysis/files/8102308/Outcomes.by.Month.pdf)

This table was used to create a line chart to show outcomes of various campaigns based on launch date.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/99691015/154804175-6387b702-62c1-44d2-b566-0b800c36a2eb.png)

2. Outcomes Based on Goal Amount:
A table with ranges of goal amounts was created and populated using the COUNTIFS function. This counted successful, failed and canceled campaigns based on the total amount of the original goal.  


[Based on Goal Amount.pdf](https://github.com/Rpisipati2022/Kickstarter_Analysis/files/8102315/Based.on.Goal.Amount.pdf)

This allowed an analysis of campaign outcome based on original goal amount per the line chart shown here. 

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/99691015/154804335-e6cc9cc7-f61f-4d50-8a5d-acca1bcfddec.png)

## Challenges
-	The Linux time stamp is not an intuitive number to work with. One needs to look up how to convert this to a standard date:

[Linux Timestamp.pdf](https://github.com/Rpisipati2022/Kickstarter_Analysis/files/8102319/Linux.Timestamp.pdf)


-	The COUNTIFS function is very elegant and an effective way to select data that exactly matches specific criteria. One should be careful with the format, especially in copy/pasting formulae over a range of fund-raising goals. It is recommended to conduct a separate check. e.g. count all the “successful’ campaigns and verify that this total is the same as the sum total of the various successful campaigns over specified goals targets. 

## RESULTS
Theater outcomes by launch date:
-	There appears to be a strong correlation between when a campaign is launched and the potential for its success: campaigns launched in July seem to succeed at a rate 2X those that start in other months. A separate analysis of successful outcomes by month showed that June/July generally had lower goal amounts which coincided with the observation that lower goal campaigns generally succeeded.


[Goan and Month.pdf](https://github.com/Rpisipati2022/Kickstarter_Analysis/files/8102324/Goan.and.Month.pdf)

-	Campaigns that failed, on the other hand, do not seem to be time dependent. This indicates there may be other reasons why they failed to raise their goal amount.

### Potential Limitations of the Database:
Potential Limitations of the Dataset:
-	Most of the data is US generated, of which two cities account for the majority share, i.e. may not reflect an unbiased view of the GB fundraising infrastructure
-	A common watch out to creators is to be careful describing their projects – they may be copied by others and they may not be first to market
-	Theater accounted for only 12% of all successful pledged dollars in KS, of which plays accounted for ~7%, i.e. this is a relatively small slice of the total pledged amounts and is influenced by other, larger campaigns

### Additional Graphs/Tables:
- the analyses showed that most successful outcomes occured with campaigns that kicked off in the June?July time frme as well as the fact that total goal amounts in the $5000 range tended to be most successful. Analyzing the data to validate this correlation would provide additional insight into when a campaign should be launched and the goal amount to ask for.
