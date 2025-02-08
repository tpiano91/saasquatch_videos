# Exploratory Analysis for Saasquatch Videos

##### This project was completed as part of a technical assignment at a recent job interview. 
##### In this project, I conduct a preliminary exploration of a fictitious online video streaming service KPIs. This preliminary analysis will then serve as a foundation for future business questions, which I will be exploring and answering in future projects.
##### This ReadMe outlines the steps to my analytical process in my preliminary exploration and first chosen business question. 

# Project Overview

### Premise
##### You're an analyst for "SaaSquatch Videos": a B2C subscription based video streaming service
##### Conduct an exploratory analysis of the data and present insights to a chosen business question

### About "SaaSquatch Videos"
##### Saasquatch Videos Hosts Three Brands:
###### Dare Network: For Adults
###### Playground Prime: For Children
###### Mosaic: For General Audiences
#### Mosaic is a recently launched brand
#### Dare Network has been outperforming Playground Prime in various metrics, most notably in:
###### Trial to Subscription Rates
###### User Engagement

### Chosen Business Questions
##### Why has Dare Network been outperforming Playground Prime in various KPIs?
##### Can Dare's success be replicated in the other two brands?
##### What strategies can SaaSquatch Videos' teams use to drive up numbers in the other brands?

### Datasets
##### The dataset consists of four tables: Leads, Trials, Cancellations and Watched Videos
##### Table 1: Leads
###### Records of people signing up for email campaigns, called "Leads"
###### Leads offer free teaser material to entice potential customers to sign up for a free trial subscription period
##### Table 2: Trials
###### Records of trial periods
###### A trial period is mandatory before a user can subscribe
##### Table 3: Cancellations
###### Records of users canceling their subscriptions
##### Table 4: Watched Videos
###### Daily summary of watched videos by user
###### Includes details such as: video genre, which brand the video is from, etc.

### Steps to Analysis
##### Step 1. Initial Exploration
###### Explore each individual table and record initial insghts
###### From the initial insights, note potential areas and business questions to explore
##### Step 2. Choose a Single Area of Focus (Dare's Success Factors)
###### Conduct Statistical Analyses
###### Create Visualizations for a Presentation
##### Step 3. Final Recommendations and Insights
###### Compile insights into a presentation
##### Step 4. Suggest Additional Areas to Research and Questions to Answer

# Initial Exploration and Choosing a Business Question
##### In this step, I explored each of the four tables individually. By creating visualizations and noting preliminary insights, I noted possible business questions to focus on.

### Table 1: Leads

![visual_1](visualizations/brand_counts.png)

##### "Dare Network" and "Playground Prime" have similar a number of leads. They both have far more leads than "Mosaic".

![visual_2](visualizations/brand_performance_over_time.png)

##### "Mosaic" is likely a new brand, as they had no leads until July 2024. This likely explains why they had far fewer leads than the other two brands
##### "Dare Network" and "Playground Prime" have had declining leads from March/April through July/August. 
##### "Playground Prime" shows the most extreme fluctuations - maybe caused by seasonality.

![visual_3](visualizations/month_emailed_counts.png)

##### The number of total leads fluctuates much less than individual brands (particularly the two leading brands)
##### July/August showed a healthy number of leads, despite the two leading networks ("Dare Network" and "Playground Prime") having very low numbers in those months

### Table 2: Trials

![visual_4](visualizations/campaign_brand_distribution_horizontal.png)

##### Each brand had one Lead campaign that was vastly more successful/popular than all of their other campaigns

![visual_5](visualizations/trials_per_brand.png)

##### "Dare Network" has by far the most number of trials. This is interesting because "Playground Prime" has a far lower number of trials despite having a similar number of leads. This requires further research. Possible reasons/explanations include:
###### Do more "Dare Network" Leads convert into Trials?
###### Does "Dare Network" attract more people to sign up for trials without a lead campaign?
