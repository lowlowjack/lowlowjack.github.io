---
layout: post
title: "Hiring: A more in depth look at the interview process"
subtitle: "Part 2: Examples"
tags: [data science,hiring]
author: Jack Low
share-img: "/assets/img/hiringflowdiag.jpg"
share-description: "A case study on the hiring process"
---

As I discussed previously [here](https://lowlowjack.github.io/2024-08-20-hiring-a-lesson-to-avoid-headaches/), I believe that hiring the right person was quite important. So how would you decide to  hire the person given the circumstances or not? I’d like to go through my thought process in a case study which can maybe shed some light in terms of how I would look at things. 

## Interview process 

Let’s suppose as a thought experiment we’re hiring these several roles for an analytics team in some industry. This thought experiment is meant to reflect a hypothetical company, not any real life situation. 

- Data analyst for an anomaly analysis role in the loans team (LOANS). They would be working on detecting anomalies within the system and analyzing root causes of issues in our loans systems.
- Data scientist for an operations role (OPS), they would be working on a Gen AI project to build a chatbot that would be optimal for the customer experience for customer complaints regarding non reception of products. 
- Data scientist for user segmentation in LOANS team. They would be building risk models that describe the propensity of a user with x features to commit fraud and to escalate these segments up to stakeholders for further processing.  

Team currently has
- LOANS: 1 data scientist, 4 data analysts 
- OPS:   2 data scientists. 

## Pre interview 

There is a data scientist candidate coming in today for an interview, but what should I be thinking when hiring them? What does our company need at the current moment? My thought process behind whether to hire or not can be summarized as below, although it isn’t strictly numeric.  

![Hiring priority diagram]( {{'/assets/img/hiringflowdiag.jpg' | relative_url }} "Hiring flow")

I start with a baseline of 5, (that’s my default belief, but it can adjust depending on the situation), and then adjust both ways as above. So in the example, above... 

Yes. According to the manager, the data analysts in the loans team are overloaded trying to detect anomalies/bad actors and we are quite close to being overloaded by how many  cases there are. I’m not sure they can bring their data analysts off the job and still not have issues trying to cope with their workload: it would take 1 year for them to get the correct skill sets (+1 - **reallocation**: LOANS).  The manager also wants to make sure their existing data analysts can do other work besides reacting to the status quo (+2 - **importance**: LOANS). In the meantime, there is also a big push from other functional groups to try to get the Gen AI project finished, as there is already some buy-in from the high levels and the new data scientist for the operations role would be replacing one person who is leaving (+2 - **importance**: OPS). Their immediate priority is to push this project over the finish line. 

I’ve talked to the managers of both teams, and we’ve come to a collective agreement that any data scientists that can be considered for both departments should have higher priority in the loans team. The reasoning we came to was that if I do not hire the data scientist for the loans team by 3 months, then, the potential issue of credit and fraud risk not being taken care of will escalate to the rest of the organization which will negate any gains from the operations project (+1 - **time to hire**: LOANS). The data analysts are also quite stretched and are at potential risk of burnout. While the cost of not finishing the Gen AI project quickly is present, it can still be finished by reassigning and reprioritizing the project to the one data scientist in operations if need be (-1 - **reallocation**: OPS). If you’ve been keeping track, you would have noticed that LOANS team has a lead in terms of priority here. I will try to hire for both roles, and it’ll depend on the candidate to where I think they’ll be best suited as well. 

## Beginning the interview

The clock strikes 4, and the candidate enters. We make our rounds of introductions as I see our candidate. They are quiet, but seem confident and tell me that they know a few friends working here, and we have a quick chat. Not too long after, the interview starts, and I have a panel with me: another senior of the analytics department and someone from the hiring team. *My first impression of them is that this could be good as I don’t see many confident data people around.* 

> Interviewer: So tell me about yourself…. 

We get right into it and they discuss more about their experiences so far. They seem to be very fluent in terms of describing what the initial problem they had solved so far was, and how they went about trying to create the model and how they deployed their solution to production from end to end. They also measured how much of an impact the model had, and when I quizzed them about it, they did give reasonable logic on how the estimates were derived. So far, *I am impressed as they are able to stand out from the crowd by showing their impact to their company.*

I asked them more on the specifics, on what else they explored, but they used this model more as a standard industry benchmark rather than trying to explore other models to get the solution out quickly. I liked that they prioritized value here, although I wished they could have explored a bit more here. Overall, not a big sticking point. A bit later, I tried to highlight the following in their resume.  

> Interviewer: You mentioned that you had experience in implementing Gen AI solutions. Can you tell me more about that? 

We had a very brief chat about the subject for about 3 minutes. They were at the beginning phase of the project exploring available external data for the RAG component, and so they didn’t get much involvement with the architecture. For me, *this moves my intent for them towards the LOANS data scientist a bit more strongly, given they have more flexibility as a candidate overall rather than specialization in one field that may be more useful.* 

The candidate then proceeds to demonstrate their other skills during the interview.  We have a great chat, and they proceed to do a good presentation of their take home assessment. As in any other meeting, *the candidate had a strong sense of purpose in terms of what they wanted to show and they had prepared beforehand for that.* 

At the end of the interview, before they leave, they ask this question:

> Candidate: Can you tell me more about your company’s culture? 
>
> Interview: Well…

If you don’t know how to answer this question, learn it ASAP. You probably need help, or you should not be in this position. There are many people who can give you a differing definition of what company culture is, and I hear a lot of talk on needing soft skills. And all of that is to try to answer this question of cultural fit. My working definition that I use is how I think the people in the company work as a whole, and in particular, how the candidate's future team will be working.

- Depending on the size of the company it can be very different. How are things communicated? How fast do things move? 
- Can they be done directly, or are there proper channels? 
- Are we free to ask questions and what kind of answers do we get here? 

I’d like to think that we’re not hiring sheep that will just follow along with everything. Then again, what are your chances that you call on the apocalypse?  

[![Wake UP SHEEPLE](https://imgs.xkcd.com/comics/wake_up_sheeple.png)](https://xkcd.com/1013/)

Getting along at work is probably ideal. If one manager would fit the candidate, but not get along with another, the answer is still usually no. (assuming both managers have established themselves) We are looking to hire for an overall fit and the issue is bound to surface sooner than later, and it’s worth to discover that it’s not going to work early rather than down the line. Seek to hire for an organization, then a role. If they fit the right culture, even if they don’t have the full skill sets, they can probably figure out the last leg of it. Skills can be learnt! 

I give them an answer, and we call it a day. The candidate leaves the room and we move to discuss our thoughts. It was quite a good interview and ultimately, that is what a good interview should do: **leave a good impression of the candidate on the hiring managers.**

## Final thoughts 

This candidate today had some skills in implementing Gen AI, but also has done some product work which I think can translate over to the loans side. Based on the above, if they have most of the skill requirements and fits the culture, I would be willing to accept them for the fraud team first, unless they’re exceptionally skilled in Gen AI, in which case, I can consider different arrangements with the teams. So how did the candidate do?

| Question (high-level) | Subtopic | Details |
| ----------- | ----------- | ------- |
| Do they fit the culture? | Do they have evidence from working experience to suggest that they can fit into the culture? | They were able to present their solution in production and answer questions about how it would impact the business well. This suggests that they could explain the solution well with non technical folks. I would like them to be a bit more explorative in their solutions, but that is not too big an issue.|
||When given an unseen question, how did they respond to it? How did they work with you to answer the questions?|During their take home test presentation, we noticed that they made a small error in the assessment. They managed to pick it up after a few hints and gave a solution on how they would address it for the future. |
|Do they meet the hard skill requirements?|What evidence did they give?|They had some experience in Gen AI and in deployment of solutions in production. They could give reasonable estimates that were sensible. |
||If you ask them about subtleties of skills, can they respond and think about it?|They discussed the intricacies of deploying their solution to production and some of the things that they had to fix that were not anticipated. (e.g data drift, model prediction speed)|

Based on the above, the candidate seems like they would fit in. The panel has a discussion and comes to an agreement that we’ll hire the candidate. We’ll give an offer and see how it goes. 

*** 

While we can’t guarantee that the person hired is right, we can do our best to make sure that they are the best. By sharing some of the process, I hope that both candidates and hiring managers can come to a better understanding in terms of what each other might need. In terms of my process, I don’t think my systems are the definitive end all, and I think we can come up with a better system that allows us to decision better and maybe one day, someone will figure it out. For now, to candidates looking out there, good luck and to hiring managers, hope that you’ll find your shining star soon. 
