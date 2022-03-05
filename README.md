# Kickstarting with Excel

## Overview of Project
Our client is looking to launch a Kickstarter campaign to fund a theatrical play and is looking to us to create an analysis of some data provided by Kickstarter.  We are going to use Microsoft Excel to perform this analysis.
### Purpose
To analyze provided Kickstarter data in order to glean insights and use that information to help our client decide on a funding goal and launch date that would have the best chance of being successful. 
## Analysis and Challenges
Based on the findings, we can state that there are levels of funding goals that correspond to positive outcomes, and that there is an optimal time of year to launch a campaign.  
### Analysis of Outcomes Based on Launch Date
Based on the analysis of the outcomes based on Launch date, we can see that most successful Kickstarter campaigns are launched in May and June, before trailing of towards the end of the year, with a small spike in October.  We can see that the failed campaigns curve is much flatter, however it does have a similar spike in October.  We need to look at another factor for trends.
### Analysis of Outcomes Based on Goals
We can see that at up to a goal of approximately $5000 over 70% of campaigns are successful, and then it starts to drop of pretty dramatically from there, until we hit the $35,000 to $45,000 threshold where successful spike back to 66.7% success before dropping off again.  This is, however, a much smaller group of only 9 campaign launches in the $35-45k range, versus a total of 529 campaign launches under $5000 so perhaps we should not put too much weight behind this spike in data.  Interestingly, the failed outcomes curve is a mirror image of the successful curve, and there are 0 cancelled campaigns in this dataset.
### Challenges and Difficulties Encountered
During the analysis, the biggest challenge I came across was using the COUNTIFS function.  The information provided was a great start, however when needed to add the range of funding goals (eg 1000-4999, 5000-9999) I had to do some of my own research and experimentation.  After some time, I was successful.  Having to manually complete the Outcomes based on Goals chart was good practice and helped re-enforce the learning. 

Here is my code: =COUNTIFS(Kickstarter!$D:$D,">=1000",Kickstarter!$D:$D,"<=4999",Kickstarter!$F:$F,"successful",Kickstarter!$R:$R,"plays")

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The best time to launch a Kickstarter campaign is in May or June, with the worst time being November/December.

- What can you conclude about the Outcomes based on Goals?

The goal for the Kickstarter funding should not exceed $5000 for the greatest chance of success.

- What are some limitations of this dataset?

The data does not include any reviews of the successful and failed plays, which could add additional insight.  Also, the Kickstarter data is quite old, with the most recent campaigns dating back to 2017.  I would have liked to have more recent data.

- What are some other possible tables and/or graphs that we could create?

Creating a chart based on the total number of successful and failed will help us visualize the data to give us insight on some spikes in the Outcomes based on Goal chart we created, essentially explaining that the spike at $35-45k was a bit of an anomaly when looking at the total number of projects.  In fact, it barely registered at all.  I have included this chart in my resources, titled: Number of Succeddful vs. Failed
