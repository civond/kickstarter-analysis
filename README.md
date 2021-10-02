Kickstarting with Excel (Crowdfunding Analysis)

<h2>Overview of Project<h2/>
The purpose of this analysis was to review and visualize various statistics on how different kickstarter campaigns fared in relation to their launch dates and funding goals.

<h2>Analysis and Challenges<h2/>
<br/>
I performed the analysis by filtering the raw kickstarter data and placing it in a pivot table. Excel functions such as =COUNTIFS() was also used to count the number of campaigns of a certain type.
Fortunately when performing this analysis, I didn't run into many problems. 
However, the most trouble that I had was with using the COUNTIFS() function to count the number of campaigns that goals between two dollar amounts (ex: goal $5000-$9999).
I initially assumed that I could use the function like so: 
<ul> 
<li> =COUNTIFS(Kickstarter!$D:$D,">=1000","<=4999") <li/>
<li> =COUNTIFS(">=1000",Kickstarter!$D:$D,"<=4999") <li/>
<ul/>

<br/> However, I soon realized that I had to do the lower and higher bound indivdually (like so: =COUNTIFS(Kickstarter!$D:$D,">=1000",Kickstarter!$D:$D,"<=4999")


<h2>Results<h2/>
<br/>
Referring to the "Theater Outcomes Based on Launch Date" figure, the failure rate for theater projects is overall the same throughout the year.
May appears to be the best time of year to begin a theater-related kickstarter. In the same figure, we can also see that December has the lowest success rate
<br/>
Referring to the "Outcomes based on Goals" figure, we can see that if the goal of the kickstarter campaign is over $45,000 USD, 
then the success rate begins to drop significantly.
<br/> Some limitations of this dataset is that it contains US kickstarter projects as the largest portion. 
Other countries don't have the same amount of representation. For example, Singapore only has one project, and the UK has 366, compared to 1651 for the US.
<br/> Other potential figures that we could make is success rates for a given parent category per country, etc.