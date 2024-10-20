---
layout: post
title: "Peaking into the SEA Data Landscape"
subtitle: "Where are we as a data field in Malaysia?"
tags: [data science]
author: Jack Low
share-img: "/assets/img/projection_img.png"
share-description: "A study into the state of recruitment for data roles in Malaysia and Singapore"
---

Back in 2022, a quick [study](https://towardsdatascience.com/data-to-engineers-ratio-a-deep-dive-into-50-top-european-tech-companies-58abc23e36ca) was done in terms of the data to engineer ratios in European companies and I found it quite insightful in terms of how it gave a picture of the data space. The natural extension to that question then was what about Malaysia now? I was curious to see what if we try to extend it and understand what is the landscape of data in Malaysia: where do we stack up compared to the rest of the world and what can we, both as professionals and companies, learn from these findings and use it to improve the data ecosystem in Malaysia?

## Sampling and Analysis

To get a clearer picture, we sampled and analyzed around 300 different job descriptions from  Glassdoor, LinkedIn, and JobStreet. The idea being that if a company has a large data expansion plan, they should reflect that presence on the job boards for data roles relative to other companies, which allows us to assess the general state of data roles in general without knowing too much specifics. Singapore serves as a control to measure how Malaysia stacks up in terms of data readiness within the region. I've included the notebook with analyses details here. 

In interpreting the results, we used the data to engineer ratios as above. A higher likelihood ratio implies companies are more actively seeking data roles, although prolonged job postings due to a shortage of candidates may also skew this number. Let's make a hypothesis in terms of what we expect to see:

1. We should see that Singapore should have higher demand for data roles compared to Malaysia. 
2. There should be a prevalence of data analyst roles in Malaysia compared to more advanced engineering or scientist roles. 

Now, let's see the data. 

![Data from Three Regions](/assets/img/fl_capture.jpg "Data from Three Regions")

From the data:

- **Singapore** has a higher engineer-to-data ratio compared to Malaysia with more balanced hiring across data scientists, analysts, and engineers. It is about on parity compared to Europe of 2 years ago. 
- **Malaysia** shows a skew towards data analyst as expected. What is surprising is that the engineering roles is also quite developed showing similarities to Singapore. 

The heavier emphasis on analysts and engineers in Malaysia suggests that we are in the early stages of the data industry in Malaysia in a few different senses. 
1. We do not have data enablement activated given the large demand here. We should also expect that data analysts may function as a pseudo data engineering double for companies who have not reached the maturity level yet.
2. Given the lack of data scientists and prevalence of analysts, it is possible that most companies do not even have a strong form of knowledge on what to even do with their data.  Data enablement might be the first step for them then to understand their potential. 

The next question to answer is is this state of industry universal among all companies or not? We should see that the gap compared to Singapore is smaller for bigger companies in Malaysia who are more mature compared to smaller companies and have a generally higher demand for data roles. Surprisingly, the answer seems to suggest maybe not.

<figure>
    <img src="/assets/img/projection_img.png"
		width="650" height="450"
         alt="Gap by different company sizes">
</figure>


 The graph shows that while **Singapore** leads in all categories, Malaysia’s gap widens as companies grow larger. It appears that large companies in Malaysia may be at the stage where they have a higher need of guidance on data enablement. We also try to simulate what happens if we match Malaysia's demand to Singapore for small companies given they have the smallest gap (yellow curve). We see that there is still a gap (red region) which indicates a possible shortage in supply for mid-size companies that is driving larger data to engineer ratios in Singapore. This seems in line with the narrative from Singapore that there are [role shortages](https://www.morganmckinley.com/sg/article/skill-shortage-impacts-technology-growth-in-singapore) there, and that even with high government intervention, it has not been able to keep pace with the demand for roles. Given large companies in Malaysia are still at the stage where data enablement or strategy is still premature, we predict that the industry will find a much larger of shortage of skilled workers in a few years time. 

***

In addition to looking at data to engineer ratios, we can also look through textual analysis of job postings to identify common hard and soft skills required for data roles in Malaysia. For the most part, they are not very different compared to other data roles globally. 


| Role           | Skills                                                            |
| -------------- | ----------------------------------------------------------------- |
| Data Analyst   | Excel, PowerBI, Tableau                                           |
| Data Scientist | Excel, Tableau, PowerBI, ML frameworks (Tensorflow, PyTorch), AWS |
| Data Engineer  | AWS/Azure, Spark, Hadoop, Kafka, Java                             |


Given the young data landscape, we do see that most data analyst roles in Malaysia encompass a generalist mindset where the engineer and scientist roles have more specialization. The hope is that as we mature, we will move towards a state where scientists and other research based professions become more common. 

![Specialization of roles](/assets/img/specialization.jpg "Specialization of roles")
*Current data analyst roles are mostly mixed, and will specialize*


What was an interesting addition to the job description was that Singapore's job postings had a notable trend toward **data + industry specialization**—where roles are increasingly focused on applying data to sector-specific problems. So what do all these findings tell us about the future of data in Malaysia?

## The Future of Data in Malaysia

Malaysia’s data landscape is still young, but I also do see the potential here. 

- The main issues facing Malaysia is data enablement and a lack of data strategy. This would be an area for data professionals to focus in terms of how data could be used to create value for business. 
- We will see an increase in specialization from the data analyst field, and existing data analysts will need to do the same to remain competitive. Some areas which I think could hold future potential could be
	- Data Engineering: As clearly mentioned above, there is an increase in demand of data engineers and this will only grow as more companies are preparing the transition. 
	- Operations Research: With such a large logistical market, it makes sense that we will need to study the best way to organize these systems. 
- With Singapore already experiencing a shortfall of senior data professionals, Malaysia will likely face similar challenges soon if it has not already. My advice to companies with data teams is to manage well, keep staying ahead and innovating on the data trends, otherwise, you'll find yourself without a team soon. 

With the growth of investment into data centres in Malaysia, some of the folks I've spoken to believe and have a renewed hope for the future of a data career in Malaysia. There are many steps that need to be taken before we have a strong data culture in Malaysia, but this general enthusiastic atmosphere does remind me of something. If we recall Fusionex before their incidents, they used to be considered one of the major players of AI in Malaysia many years ago. While there are many lessons to be learnt from there, my takeaway is that even for Malaysia, there still is a large potential for data that is still unrealized. The question is, who will fill that gap and I am no doubt excited to see what the future holds for us here.  

## References

1. [Data to engineers ratio: A deep dive into 50 top European tech companies](https://towardsdatascience.com/data-to-engineers-ratio-a-deep-dive-into-50-top-european-tech-companies-58abc23e36ca). Mikkel Dengsøe
