# Optimzing Employee Training Systems

## Table of Contents

- [Scope & Goals of Analysis](#scope-&-goalsof-analysis)
- [Dataset & Overview of Data Structure](#dataset--overview-of-data-structure)
- [Executive Summary](#executive-summary)
- [Insights Deep Dive](#insights-deep-dive)
- [Recommendations](#recommendations)
  

## Scope & Goals of Analysis

ACCO Engineered Systems is a mechanical engineering company operating in Arizona, California, Florida, Hawaii, Idaho, Nevada, Oregon, Utah and Washington. Their Training and Development department contracts several Learning Management System vendors to deliver various training programs to their employees. The Learning Data Analyst position opened for applications in March of 2025 detailing involement in the optimization of LMS and content delivery. I obtained this data set as an applicant to the position and delivered my insights to the Training and Development Team in my first-round interview. 

The **main objectives** of this analysis are to:
1. Identify associations betweeon Outcomes and Training Module Characteristics.
2. Investigate patterns in Vendor and Training Program offerings.
3. Optimize Vendor Spending.

## Dataset & Overview of Data Structure

ACCO generated a Technical Assessment data set containing 24 original columns of 150 rows. Each row represents a training module assigned to an employee, detailing assignment and training module details. 

To help explain missing data related the "Completion Date" column, I created a "Days Overdue" column that pulls information from the "Completion Status," "Assignment Date," and "Due Date" columns. Data from 25 columns were used in the analysis.

Below is the data field summary:
<div align="center">
 <img width="631" alt="Image 1" src="https://github.com/user-attachments/assets/2d66561f-8dde-441d-a57c-5fd29c8b22a9" />
</div>


## Executive Summary


## Insights Deep Dive

### Training Outcomes & Ratings

#### Training outcomes are not predicted by a single Factor

<p align="center">
  <img src="https://github.com/user-attachments/assets/fc73e042-434d-42b2-bf4c-9ef570f24397">
  <img src="https://github.com/user-attachments/assets/1256b51c-df05-482c-9af9-db99cbde91c5">
</p>

Outcomes such as Assessment Score, Engagement Score, Training Feedback Rating, and Cost per Learner vary substantially across vendors. While some vendors demonstrate a favorable *cost-performance balance*, **others charge more without delivering** better outcomes.

* Skillsoft and BizLibrary emerge as **cost-efficient** vendors, with *lower-than-average costs* ($223.12 and $218.98, respectively) and **above-average engagement** (4.9 and 6.2).
* Ninjio and Traliant, two of the most used vendors, have *costs above the overall mean* ($241.09 and $297.62) but *do not lead in any performance metric.*
* LinkedIn Learning has one of the **highest costs per learner ($325.17)**, yet its assessment scores and engagement are **below the grand average.**


Spending more does not correlate strongly with better outcomes. Correlations between cost and assessment score (~0.20) and engagement (~0.05) are weak. This suggests that vendor selection should be guided by cost-effectiveness, not brand familiarity or pricing.

#### 

<p align="center">
  <img src="">
  <img src="">
</p>



### Vendor Saturation 

#### Reducing Vendors will Optimize Spending & Training Outcomes

<p align="center">
  <img src= "https://github.com/user-attachments/assets/c1952622-c219-4152-8d26-4644a7d7a627">
  <img src="https://github.com/user-attachments/assets/a670bb44-d7c7-4b9d-b09b-500c565cf600">
</p>

Over a two-year span, Traliant and Ninjio accounted for a combined 37% of all assignments. These vendors also operate across the most locations and quarters.
However, deeper analysis reveals that this dominance is largely due to their coverage of mandatory training topics rather than superior training quality.

* Ninjio leads in Cyber Security, while Traliant dominates Harassment Prevention. These two areas collectively account for the majority of their assignments.
* Both vendors are offered in 5+ locations and are active across multiple quarters, particularly **Q2 and Q3, where overall sales peak.**
* Despite their prevalence, neither vendor excels in key training outcomes: their average engagement scores hover at or below the dataset mean, and feedback ratings remain neutral (2.9–3.1 out of 5).

Current vendor saturation reflects compliance needs, not strategic effectiveness. A strategically curated vendor selection, focused on cost-effectiveness and content quality, could enhance both outcomes and ROI.

#### 

<p align="center">
  <img src= ">
</p>

<p align="center">
  <img src="" >
  <img src="">
</p>


### Vendor's Sales by Location

#### Vendor Drives Sites' Outcomes

<p align="center">
  <img src= "">
</p>

<p align="center">
  <img src="">
  <img src="">
</p>


#### 




## Recommendations
**Strategic takeaway:** 

** **
**Implication:** 

**Recommendations** for :
1. 
2. 

** **
**Implication:** 

**Recommendations** for :
1. 
2. 

** **
**Implication:** 

**Recommendations** for :
1. 
2. 
