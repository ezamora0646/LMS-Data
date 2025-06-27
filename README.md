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
1. Identify associations between KPI and Training Module Characteristics.
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
* Vendor impact varies widely: Higher cost does not consistently translate to better performance.  For instance, BizLibrary and Skillsoft deliver *above-average* assessment scores (78.0 and 81.2) and engagement scores (6.2 and 4.9) at **costs 20% below the average** ($218.98 and $223.12 vs. $278.77). In contrast, Coursera and Go1, with **average costs over $300** per learner, deliver *lower than average* assessment scores (69.7 and 72.5) and feedback ratings (3.4 and 1.6).

* Saturation does not equal effectiveness: Two vendors—Traliant and Ninjio—account for 37% of all assignments, active across 5+ locations and multiple quarters. However, their engagement scores (4.9 and 5.5) and feedback ratings (3.1 and 2.9) sit near or below the overall average, indicating benefit from continued performance tracking to motivate their continued use.
  
* **Location outcomes are vendor- and delivery-dependent:** Reno, which balances hybrid, online, and instructor-led formats, records the *highest engagement (5.4) and feedback ratings (4.0).* It sources from vendors like Traliant and BizLibrary, whose training programs span key content areas. In contrast, San Leandro, relying heavily on BizLibrary and online formats, sees *engagement dip to 3.8 and feedback fall to 2.2.*

**Key Takeaway**
Training outcomes are not driven by a single factor, but by the interaction between cost, vendor selection, and delivery format. To boost ROI and learning effectiveness, organizations should prioritize cost-efficient, high-performing vendors and optimize delivery strategies based on site-level needs and performance data.


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


Spending more does not correlate strongly with better outcomes. Correlations between cost and assessment score (~0.20) and engagement (~0.05) are weak. This suggests that vendor selection should be guided by cost-effectiveness, not brand familiarity or pricing. This weak correlation holds even among the most expensive vendors—some deliver moderate to strong outcomes (e.g., Infosec, Skillsoft), while others (e.g., Coursera, Go1) underperform. This highlights the importance of tracking vendor-specific ROI.

<p>
  <br>
</p>

### Vendor Saturation 

#### Reducing Vendors will Optimize Spending & Training Outcomes

<p align="center">
  <img src= "https://github.com/user-attachments/assets/c1952622-c219-4152-8d26-4644a7d7a627">
  <img src="https://github.com/user-attachments/assets/a670bb44-d7c7-4b9d-b09b-500c565cf600">
</p>

While Traliant and Ninjio account for a combined 37% of all assignments, this reflects their critical role in delivering mandatory content (e.g., harassment prevention and cyber security) across multiple sites. These vendors also operate across the most locations and quarters.
Their performance is consistent with dataset averages, and their breadth of delivery formats—especially hybrid—supports a range of training needs. However, their continued inclusion should be justified through ongoing outcome monitoring.”

* Ninjio leads in Cyber Security, while Traliant dominates Harassment Prevention. These two areas collectively account for the majority of their assignments.
* Both vendors are offered in 5+ locations and are active across multiple quarters, particularly **Q2 and Q3, where overall sales peak.**
* Despite their prevalence, neither vendor excels in key training outcomes: their average engagement scores hover at or below the dataset mean, and feedback ratings remain neutral (2.9–3.1 out of 5).

However, dominant vendors consistenyly outperform low volume vendors: 
* Go1, Infosec Institute, and Coursera serve few programs and locations yet report below-average outcomes in multiple metrics

Current vendor saturation reflects compliance needs, not strategic effectiveness. A strategically curated vendor selection, focused on cost-effectiveness and content quality, could enhance both outcomes and ROI.

<p>
  <br>
</p>

### Vendor's Sales by Location

#### Vendor Drives Location Outcomes

<p align="center">
  <img src="https://github.com/user-attachments/assets/491d855f-70d6-4111-991c-d8523398abed" >
</p>

Outcomes at the site level are strongly influenced by which vendors are selected and how their programs are delivered. In Reno, average engagement (5.4) and feedback ratings (4.0) significantly exceed those in San Leandro (4.2 and 2.2, respectively), despite both locations having similar average costs per learner (~$281 vs. ~$257).

The key differentiator appears to be the Content Vendor and their delivery method mix. Reno’s performance is achieved through a balanced delivery approach and selection of high-engagement vendors (e.g., Traliant, BizLibrary). The equal use of hybrid, online, and instructor-led methods appears to drive its success. This mix is associated with the highest feedback scores overall, especially for instructor-led formats (4.9 in Reno vs. 2.7 in San Leandro).

Meanwhile, San Leandro sources heavily from vendors like BizLibrary, which show weaker engagement and more limited delivery flexibility. Hybrid delivery in San Leandro yields the lowest engagement (2.0) and feedback (1.4) across any location-delivery pairing. Online training, while common, does not compensate for this gap.


Across all locations, instructor-led formats are associated with the highest assessment scores (77.6) and feedback (3.2), reinforcing the notion that delivery method, not just vendor or cost, is a strategic driver of site-level training success. However, hybrid formats perform nearly as well, with comparable assessment outcomes (74.6) and slightly lower feedback (3.1)—at a lower average cost ($258 vs. $285 per learner). This makes hybrid training a compelling value proposition.

<p>
  <br>
</p>

## Recommendations
**Strategic takeaway:** 
Vendor selection and delivery method are strategic drivers of both performance and cost-effectiveness. Current saturation patterns reflect compliance needs rather than training impact. By *rebalancing the vendor portfolio* and delivery approach, organizations can improve learning outcomes and **optimize return on investment.**


**Recommendations** for Vendor Selection and Cost Efficiency:
1. Streamline the vendor portfolio by retiring low-usage vendors (Go1, Infosec Institute, and Coursera) that *incur high costs* without outperforming widely used alternatives.
2. Continue leveraging vendors that are both widely used and competitively performing in mandatory training areas (e.g., Traliant, Ninjio)—but hold them to performance benchmarks. These vendors are essential for coverage, but ongoing evaluation ensures they don’t become high-cost defaults.

3. Establish a vendor scorecard framework that tracks performance KPIs (e.g., engagement, cost, assessment score, feedback rating) alongside usage patterns (e.g., quarters active, locations served). Use this to guide contract renewal and procurement decisions.
 

**Recommendations** for Training Delivery and Site-Level Strategy:
1. Expand instructor-led and hybrid training formats, which yield the strongest outcomes. Instructor-led training shows the highest average scores and ratings, while hybrid delivery offers comparable results at lower cost—making it a compelling value option.

2. Tailor delivery strategy by location, modeling successful sites like Reno, which combines diverse delivery formats with high-performing vendors. 

