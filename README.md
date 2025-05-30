# Exploratory Analysis for Saasquatch Videos

##### This project was completed as part of a technical assignment at a recent job interview. 
##### In this project, I conduct a preliminary exploration of a fictitious online video streaming service KPIs. This preliminary analysis will then serve as a foundation for future business questions, which I will be exploring and answering in future projects.
##### This ReadMe outlines the steps to my analytical process in my preliminary exploration and first chosen business question. 
##### To view my full presentation, please check my repository or click here: https://github.com/tpiano91/saasquatch_videos/blob/main/presentation_1.pdf

# Project Overview

### Premise
##### You're an analyst for "SaaSquatch Videos": a B2C subscription based video streaming service
##### Conduct an exploratory analysis of the data and present insights to a chosen business question

### About "SaaSquatch Videos"
##### 1. Saasquatch Videos Hosts Three Brands:
###### Dare Network: For Adults
###### Playground Prime: For Children
###### Mosaic: For General Audiences
##### 2. Mosaic is a recently launched brand
##### 3. Dare Network has been outperforming Playground Prime in various metrics, most notably in:
###### Trial to Subscription Rates
###### User Engagement

### Chosen Business Questions

##### 1. Why has Dare Network been outperforming Playground Prime in various KPIs?
##### 2. Can Dare's success be replicated in the other two brands?
##### 3. What strategies can SaaSquatch Videos' teams use to drive up numbers in the other brands?
##### In the "Initial Exploration" section, I will explain how and why I chose these three business questions

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

# Step 1. Initial Exploration and Choosing a Business Question
##### In this step, I explored each of the four tables individually. By creating visualizations and noting preliminary insights, I noted possible business questions to focus on.

## Initial Exploration

### Table 1: Leads

![visual_1](visualizations/brand_counts.png)

##### 1. "Dare Network" and "Playground Prime" have similar a number of leads. They both have far more leads than "Mosaic".

![visual_2](visualizations/brand_performance_over_time.png)

##### 1. "Mosaic" is likely a new brand, as they had no leads until July 2024. This likely explains why they had far fewer leads than the other two brands
##### 2. "Dare Network" and "Playground Prime" have had declining leads from March/April through July/August. 
##### 3. "Playground Prime" shows the most extreme fluctuations - maybe caused by seasonality.

![visual_3](visualizations/month_emailed_counts.png)

##### 1. The number of total leads fluctuates much less than individual brands (particularly the two leading brands)
##### 2. July/August showed a healthy number of leads, despite the two leading networks ("Dare Network" and "Playground Prime") having very low numbers in those months

![visual_4](visualizations/campaign_brand_distribution_horizontal.png)

##### 1. Each brand had one Lead campaign that was vastly more successful/popular than all of their other campaigns
##### 2. "Playground Prime" had the most popular campaign of all, "Cuddle Up for Cartoon Time" 
###### It would be useful later to check if this campaign launched during one of "Playground Prime's" peak months of December or March (See corresponding graph above)

### Table 2: Trials

![visual_5](visualizations/trials_per_brand.png)

##### 1. "Dare Network" has by far the most number of trials. This is interesting because "Playground Prime" has a far lower number of trials despite having a similar number of leads. This requires further research. Possible reasons/explanations include:
###### Do more "Dare Network" Leads convert into Trials?
###### Does "Dare Network" attract more people to sign up for trials without a lead campaign?

### Table 3: Cancellations
###### I did not use this table for my chosen topic, but the initial insights from this table warrant further research

![visual_6](visualizations/cancellations_over_time.png)

##### 1. There was a steep, steady rise of cancellations between December-February and June-August. Look into possible reasons.

### Table 4: Watched Videos

![visual_7](visualizations/videos_watched_by_brand.png)
##### 1. "Dare Network" shows highest levels of user engagement by far by number of videos watched

![visual_8](visualizations/videos_watched_by_genre.png)
##### 1. "Comedy" and "Reality" are by far the most popular genres by number of videos watched. Possible reasons to look into include:
###### Are users binging these videos in one sitting? 
###### Are more users watching these overall?

![visual_9](visualizations/videos_watched_over_time.png)
##### 1. There is a recent decline in user engagement (video watch time) between July-August

## Choosing business questions to explore

#### From the initial exploration and my recorded preliminary insights, there were multiple interesting possible questions to explore. I chose three business questions to guide my exploration. Other questions may be explored in future projects.

##### 1. Why has Dare Network been outperforming Playground Prime in various KPIs?
##### 2. Can Dare's success be replicated in the other two brands?
##### 3. What strategies can SaaSquatch Videos' teams use to drive up numbers in the other brands?

# Step 2. Answering the Business Questions: Exploring Dare Network's Success Factors

#### To answer these business questions, I used a variety of analytical techniques including: statistical analyses; merging tables; creating additional visualizations; creating a presentation; suggesting follow-up questions and next steps for further research. First, I discovered and recorded further contextual insights that further focused how I wanted to answer these questions:

### 2A) More Context

#### Two KPIs dominated by Dare Network:

##### 1. User Engagement: Number of Videos Watched (see corresponding bar graph above)

![visual_10](visualizations/has_converted_by_brand.png)
##### 2. Highest number of trials AND trial to subscription conversion Rate

### 2B) Insights about Video Genres

#### In order to replicate Dare Network's success in other brands, I checked out what types/genres of videos Dare Network users preferred. How did this compare to other brands, and which genres were most popular overall?

![visual_11](visualizations/videos_watched_by_genre.png)

##### 1. The most popular brands by far were Comedy and Reality, followed by Thriller and Drama

![visual_12](visualizations/popular_genre_by_brand.png)

##### 2. Dare Network's genre preferences are in line with the most popular genres across all brands
##### 3. Playground Prime's users had very different genre preferences compared to the other two brands, preferring Family/Kids, Fantasy, Documentary and Sci-Fi
##### 4. Dare Network and Mosaic's users exhibit similar video genre preferences - one could speculate/research if loading Mosaic's content with the same genres as Dare Network's could yield successful results

### Statistical Analysis: Does high user engagement (number of videos watched) correlate to high conversion rate (trial to subscription conversion)?

#### Do converted and non-converted users watch the same number of videos? 

![visual_13](visualizations/box_plot_all.png)
###### Full view to see outliers

![visual_14](visualizations/box_plot_all_adjust_outliers.png) 
###### Zoomed in, without outliers

##### 1. High presence of outliers in all groups, who watched extremely high numbers of videos
##### 2. Converted users watched more videos than non-converted users
##### 3. High Variability in User Engagement in All Groups (Highest in Dare Network)

#### Before concluding whether high user engagement really correlates to higher conversion rates, a T-Test is needed to check if these results are statistically significant

### 2C) Results of T-Test: Proved Statistical Signifance!

![visual_15](visualizations/TTest1.png) 
![visual_16](visualizations/TTest2.png) 

# Final Recommendations and Insights

### Actionable Insights

##### 1. Identify which aspects of Dare Network drive high user engagement
###### Potential Aspects that drive engagement: Content quality/type, UI/UX, marketing, personalized recommendations, interactive content, reward-based incentives etc.
###### Develop and invest in strategies to further increase engagement in all three brands
###### Determine which of these aspects can be applied to the other two brands (for example, content such as reality or thriller may not be appropriate for Playground Prime but may be for Mosaic)
##### 2. Why are many high engagement users not subscribing? Identify potential barriers
###### Potential Barrers to look into: UX/UI, pricing, content type/quality, etc.
###### Conduct surveys for this subgroup to inform marketing strategy or improve product
##### 3. Why did some low engagement users end up subscribing? Identify the factors
##### 4. Monitor Mosaic’s user engagement and conversion rates in the coming months (since they’re taking over the leads)

### Recommendations for Further Testing

#### For each of the actionable insights listed above, I recommend the folowing tests:

#### Experimentation and A/B Testing (Actionable Insight 1)
###### Test new strategies or content features (inspired by Dare) to increase user engagement and identifying causation instead of just correlation
###### Business Impact: 
###### Identify which strategies/features are most effective in increasing trial to subscription conversion rates

#### ANOVA for Genre Analysis (Actionable Insights 2, 3):  
##### Two Purposes
###### Determine if there are significant differences in the mean number of videos watched across genres
###### Assess if these differences are affected by conversion/subscription status
##### Potential Business Implications: 
###### Can identify if some genres are more engaging to converted or non-converted users
###### Can identify if certain content types/genres are associated with high engagement but low conversion rate

#### Outlier Analysis through Surveys (Actionable Insights 2 and 3) 
##### Can be used to confirm insights from ANOVA (i.e. why a genre might have high engagement but lower conversion)
##### Business Impact
###### Qualitative insights on why outliers (users with extremely high engagement levels) don’t convert

#### Logistic Regression:  Predict User Conversion (Actionable Insights 3 and 4)
##### Identify key factors (genre, brand, number of videos watched, etc.) that increase likelihood of conversion
##### Measures how strongly each variable (like each genre) is associated with conversion via correlation coefficient
##### Business Impact
###### Resource Allocation: spend more money on content type that is more likely to get more subscriptions
###### Running regressions for each brand may yield insights specific to each brand (recommended)
###### Cohort Analysis for Mosaic: add a “cohort” variable for each user and see its’ correlation to conversion



