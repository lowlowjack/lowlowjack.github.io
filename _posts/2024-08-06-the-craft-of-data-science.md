---
layout: post
title: The craft of data science 
subtitle: A discussion on data analysts vs data scientists
tags: [data science]
author: Jack Low
---
Let’s observe this trend on the relative popularity of the following search term on Google from 2004 onwards. 

<script type="text/javascript" src="https://ssl.gstatic.com/trends_nrtr/3807_RC01/embed_loader.js">
</script>
 <script type="text/javascript"> 
 trends.embed.renderExploreWidget("TIMESERIES", {"comparisonItem":[{"keyword":"data science","geo":"","time":"2004-01-01 2024-08-06"},{"keyword":"data analytics","geo":"","time":"2004-01-01 2024-08-06"},{"keyword":"data analysis","geo":"","time":"2004-01-01 2024-08-06"}],"category":0,"property":""}, {"exploreQuery":"date=all&q=data%20science,data%20analytics,data%20analysis&hl=en","guestPath":"https://trends.google.com:443/trends/embed/"});
 </script>

While other data related terms have been constant over time, we see a huge growth in data science starting from 2013-2014, overtaking data analytics significantly. When I get asked by many aspiring data analysts what their future goal is, it is to become a data scientist.

If we go by some articles that would claim that data scientists build machine learning, whereas data analysts would clean data and do more of the usual reporting to business, that implies a basic, but flawed understanding to what actual data science entails: that data analysis would eventually make way for data scientists as AI and machine learning is the in thing now. I have never been able to reconcile this weird difference as I feel that the distinction is to some extent artificial and hiding a larger problem. There are a few ramifications of this:

- Several colleagues who were sold on these stories on the promise of machine learning who were data analysts before switching to data scientists have found that it was not to their expectation and moved over to different roles such as AI engineering,  data engineering, or even left the field for product design and engineering.  
- On the other hand, based on my own empirical observations, data analysts in the current setting have a more descriptive role, while data scientists would have a more prescriptive role within an organization. Descriptive in the sense that questions are being asked from business stakeholders and there are expectations to find some answers to it, where prescriptive would imply a sort of independence to find answers about the data and tell it upwards instead. 

One could imply because of this that data scientists should work in more strategy related areas, and hence, they should be more senior, but this would work only if an organization has or needs data scientists in the first place; just as more advanced data analysis, (which may involve modeling), about whether or not we have too much risk within a financial ecosystem was traditionally a risk analyst responsibility. 

In some sense, the narrative is incomplete on what defines this gap. Looking back at when data science started to truly take off in the late 2000s and early 2010s, there are a few things that came together. 

- Deep learning was repopularized about this time due to seeing success via higher computer resourcing here. AI research was heavy on the use of statistics. 
- The world became increasingly more digital, data had a higher inter-connectivity. Having big giants such as FAANG back then also helped and big data was a buzzword back then. (if you look at the trends now, it’s fallen off significantly and evolved)
- There was a strong association of data science to statistics and that there was a possibility of solving ‘big data’ problems with it. 

With all the collective interest in the field, there was an explosion of what skills a data scientist needed to focus that differentiated from the data practitioners at the time, particularly on machine learning and coding, but I also find this argument of skill difference to be unconvincing. While data science was seen as an intersection of the field of computer science and data analysis, when one thinks that the data analyst role had existed for a much longer time than data science has gotten popular, one could ask why the data analysts at the time were not evolving to the new trend given some of their similar experiences and skills as well.  

### What is data science?

I had not touched on the problem, but the science in the designation deserves some thought on its own if we ever have hope of solving science vs analytics. Among the earliest discussions of data analysis becoming a science came from John Tukey in 1962 in *The Future of Data Analysis*, as he considered the general lack of connection between statistics and data analysis, and that data analysis should be a study in itself. 

> There are diverse views as to what makes a science, but three constituents will be judged essential by most, viz: 
> - (a1) intellectual content, 
> - (a2) organization in an understandable form, 
> - (a3) reliance upon the test of experience as the ultimate standard of validity. 
> 
> By these tests mathematics is not a science, since its ultimate standard of validity is an agreed-upon sort of logical consistency and provability. 
> 
> As I see it, data analysis passes all three tests, and I would regard it as a science, one defined by a ubiquitous problem rather than by a concrete subject. 
> Data analysis, and the parts of statistics that adhere to it, must then take on the characteristics of a science rather than those of mathematics, specifically:
> 
> - (b1) Data analysis must seek for scope and usefulness rather than security;
> - (b2) Data analysis must be willing to err moderately often in order that inadequate evidence shall more often suggest the right answer 
> - (b3) Data analysis must use mathematical argument and mathematical results as bases of judgment rather than as bases for proof or stamps of validity.

Data science in our industry today is quite different as he envisioned. I find that a good deal of data professionals coming in nowadays are wanting in the intellectual content and critical thinking that is required and have a fear of uncertainty. Many new data analysts and scientists are too eager to explore the new tools, sold on the promises of relevancy, and enter with a lack of understanding on the reasoning and processes of said tools and fail to advance upon this shared knowledge. Where a reasonable approach to modeling could be to look for questions that are worth exploring, and then building on the problem and modeling process,  we now face a point that once models are built, there would be expectations that stakeholders would understand the end state on what to do with such a model rather than the model itself being a basis of judgment and insight into the problem. But when neither analysts or scientists can provide a correct sense of making sense of uncertainty, there is no data science in the first place, skills present or not. 

Take for instance, the conduct of exploratory data analysis which may not be necessarily done with correct intent. A shallow exploration would attempt to normalize or scale the data, where a deeper analysis might look into if there are missing key features required for the model that we should explicitly surface, or address the fact that a different model is required for such distributions of data, or explain the fact why feature scaling is appropriate in the first place. Scaling the model might improve the AUC, but if the assumptions on the model are incorrect in the first place, there is a much bigger problem to solve. 

### Realistic approaches to the future

You could argue the job of many data scientists is not really science, but data craft that would necessitate a pragmatic compromise of a working solution. Each situation in each company would create different environments that may seem to make generalization of the data scientist role impossible, however, I’ve found that several data scientists that may have more experience in the industry would fulfill many of the criteria that Tukey specified in their treatment of problems via tried data based solutions. Given statisticians have been around since the 1900s and are still present now, a study for the art of data can exist, so it would seem to be more a problem of consistency across our profession then. 

The problem may be that the concept of a data scientist feasibly carrying out a whole program is not feasible, and instead of the individual data scientists, we see an increase in teams within the field of data science dedicated to a strategy consisting of engineers, analysts and researchers. As a craft and science, by nature if we are to follow Tukey’s criteria, we should and are observing an aim towards specialization with designations such as Decision Science/ML Science among current data professionals, and I think, what is most interesting is how this could spell the decline of the *data scientist* designation as a whole. 

To illustrate the role of specialization and how our future could play out, we should look at the example of operations research. Operations research has been a field since the 1940s that deals with how we find optimal solutions to decision problems using data, (e.g network optimization for logistics, supply chain management etc).  I would refer to this [blog](https://leifengblog.net/blog/data-science-vs-operations-research-in-advanced-analytics/ 
) for a better comparison to it and modern data science, but one can consider the abridged table below from the corresponding blog as a reference (while the author considers the roles as separate, I would disagree and see more commonality with both). 

>|   |Data Science|Operations Research|
>|---|---|---|
>|Capability|Descriptive, Diagnostic, and Predictive|Prescriptive|
>|Business Value|Knowledge and actional insights|Optimal or near-optimal actions/strategies/decisions|
>|Quantitative Tools|Statistics, Data Mining and Machine Learning Models, Artificial Intelligence|Mathematical Modeling, Optimization Algorithms, Heuristics|
>|Paradigm|Data-Centric|Problem-Centric|
>|Project Steps|1) Opportunity statement<br>2) Data acquisition<br>3) Data exploration and opportunity reframing if needed<br>4) Model creation and Training <br>5) Iterative model evaluation<br>6) Modeling deployment|1) Identification of the problem<br> 2) Mathematical modeling/formulation of business objective and constraints<br>3) Data acquisition if needed<br>4) Iterative modeling and refinement<br>5) Modeling deployment|
>|Business Application Examples|1) Shipment volume forecasting<br>2) Delivery time estimating<br>3) Predictive fleet maintenance and fuel economy|1) Optimize stop sequence to minimize travel distance and time for pickup and delivery<br>2) Optimize network design and volume routing to minimize transportation cost|

The requirements required for an operations research analyst would overlap considerably with a modern day data scientist on closer observation and supposing we consider data science as an extension of what data analytics could be; then operations research, with its own discussions, and studies, should be a key part of the data science tool kit. For now, it remains detached, despite the fact that many data scientists could consider themselves part of that field.

In short, if data scientists are already utilizing and expanding on existing knowledge, then the role itself is ill fit, and we may need to accept the fact that our current conception of data science has become too big. In time, with the specialization of roles, we could see a resurgence of the individual fields as past research receives a renaissance similar to the ones machine learning and deep learning are experiencing. The idea of a full data scientist then too may recede in the background to other analyst roles as well, where we have teams of different decision, machine learning, and operation researchers working towards the goal of advanced data analytics, where each subfield would have a study on its own and their own sets of standards and literature.    

### What should we aim for?

As I reflect on my original perception of the descriptive vs prescriptive role of data scientists, and what differentiated the role of analytics and science, I believe we must reflect more deeply in terms of what the scientific method actually means. While I would be comfortable calling myself a data analyst, I hesitate to use the designation of scientist. Tukey’s criteria provides a starting point that we could iterate on, but also a high bar we have to consider as data science does not merely require statistics on its own and what that science will become in the future must be an active journey, differentiated not by skills, but by process. When someone asks what advice I can give  to those early in the industry, I think I would append my reply with a few more instructive ones based on what I’ve read so far. 

1. Even within specializations, we must not neglect the process: **in data science, you live day to day with uncertainty to the best path forward. To be a data scientist, you must have courage to face and question uncertainty.** 
2. Choose a specialization. As data science becomes more focused in the future, no longer is a one solution machine learning scientist enough, especially when everyone is eager to become one. 

If we are to call ourselves scientists, and reach this ideal state, we should strive to earn the name. Perhaps, the title of junior data scientist for a current data analyst would be more apt one day. 

### References 

A few more links that I think would help the discussion along and some references.  

1. [*The Future of Data Analysis*](https://projecteuclid.org/journals/annals-of-mathematical-statistics/volume-33/issue-1/The-Future-of-Data-Analysis/10.1214/aoms/1177704711.full). John Tukey.
2. [*50 Years of Data Science*](https://www.tandfonline.com/doi/full/10.1080/10618600.2017.1384734). David Donoho
3. [Data Science vs Data Analytics](https://www.datascience-pm.com/data-analytics-vs-data-science/). Data Science Process Alliance
4. [Data Science vs Operations Research in Advanced Analytics](https://leifengblog.net/blog/data-science-vs-operations-research-in-advanced-analytics/). LeiFengBlog
