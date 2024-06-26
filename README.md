# "Cyclistic"_bikeshare_project
## Data analytics case study for "Cyclistic" - bike share company.

(Images taken from istockphoto website, [license](https://www.istockphoto.com/legal/license-agreement?utm_medium=organic&utm_source=google&utm_campaign=iptcurl))

![image](https://github.com/djr111/-Cyclistic---bike-share-project/assets/58305266/70578ac4-d15f-454f-b735-6f77e3df991b)

## Introduction to Scenario:

   I am junior data analyst working on the marketing analyst team at Cyclistic, a bike-share company in Chicago.
The director of marketing believes the company’s future success
depends on maximizing the number of annual memberships. Therefore, your team wants to
understand how casual riders and annual members use Cyclistic bikes differently. From these
insights, your team will design a new marketing strategy to convert casual riders into annual
members. But first, Cyclistic executives must approve your recommendations, so they must be
backed up with compelling data insights and professional data visualizations.

About the company
   In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown
to a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations
across Chicago. The bikes can be unlocked from one station and returned to any other station
in the system anytime.
Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to
broad consumer segments. One approach that helped make these things possible was the
flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships.
Customers who purchase single-ride or full-day passes are referred to as casual riders.
Customers who purchase annual memberships are Cyclistic members.

   Cyclistic’s finance analysts have concluded that annual members are much more profitable
than casual riders. Although the pricing flexibility helps Cyclistic attract more customers,
Marketing director believes that maximizing the number of annual members will be key to future growth.
Rather than creating a marketing campaign that targets all-new customers, Moreno believes
there is a solid opportunity to convert casual riders into members. She notes that casual riders
are already aware of the Cyclistic program and have chosen Cyclistic for their mobility needs.

   Marketing director has set a clear goal: Design marketing strategies aimed at converting casual riders into
annual members. In order to do that, however, the team needs to better understand how
annual members and casual riders differ, why casual riders would buy a membership, and how
digital media could affect their marketing tactics. Moreno and her team are interested in
analyzing the Cyclistic historical bike trip data to identify trends.

   The business task in this case is to understand how annual members and casual riders use Cyclistic bikes differently. This understanding will help Cyclistic design a new marketing strategy aimed at converting casual riders into annual members. 
The goal is to maximize the number of annual memberships, as it has been identified that annual members are much more profitable for Cyclistic compared to casual riders.

![image](https://github.com/djr111/-Cyclistic---bike-share-project/assets/58305266/ab7ce891-7e48-4ffd-9919-3b9035f6dd68)


To achieve this task, the marketing analytics team needs to analyze the Cyclistic historical bike trip data to identify trends and differences in usage patterns between annual members and casual riders. The insights gained from this analysis will be used to inform the design of the new marketing strategy.

Key stakeholders involved in this task include:

Lily Moreno (Director of Marketing): Responsible for the development of marketing campaigns and initiatives to promote the bike-share program.
Cyclistic Marketing Analytics Team: Responsible for collecting, analyzing, and reporting data to guide Cyclistic's marketing strategy.
Cyclistic Executive Team: Responsible for approving the recommended marketing program based on compelling data insights and professional data visualizations.
In summary, the business task is to analyze the differences in bike usage patterns between annual members and casual riders and use these insights to design a new marketing strategy aimed at converting casual riders into annual members, with the ultimate goal of maximizing annual memberships for Cyclistic.

For this case study I will use datasets 2019_Q1 and 2020_Q1 (files archives available to download in this repository ) from public data of LLC "Bikeshare" - [link to all datasets](https://divvy-tripdata.s3.amazonaws.com/index.html).
The data has been made available by Motivate International Inc. under this [license](https://divvybikes.com/data-license-agreement).

Before starting to analyze data, I took a look on data csv files:
datasets in these files contains 350,000+ and 450,000+ observations. This is quite big dataset and best approach would be using SQL or R/Python.
As R programming language was part of the course, I decided to complete analysis and perform visualizations in Rstudio.

Attached file in repository - cyclistic_bike_share.R
Includes steps taken and documentation of the analysis
This allows to review process, code executed and replicate same process using Rscript.

The core points of analysis in R include:

- Collecting data (R already comes with default set of packages, important to remember to provide working directory path to located data files for further actions.)
- Data wrangling and combining data into a single file ("tidyverse" package for data wrangling and "dplyr" package for conflict managmeent.)
- Cleaning up data and adding data to prepare for analysis (multiple R functions for data cleaning including: mutate, summary, head, colnames, etc.)
- Conducting descriptive analysis (multiple R functions for data analysis including: aggregate, summary, mix, max, median, mean, ordered, etc.)
- Data visualisation ("ggplot2" package allows to visualize data directly in Rstudio and extract image as .PNG or .PDF file formats for further use.)
- Summary file export for further use in Tableau ( It is great to be able to present work done in other tools: Excel, PowerBi, Tableau. Created file further was used to make a viz in Tableau.)

Summary visuals created in R:

Total amount of rides by rider type:

![number_of_rides_by_weekday_and_member_type](https://github.com/djr111/-Cyclistic---bike-share-project/assets/58305266/d504bc8f-a484-43aa-a0cc-c5690d4421ef)


Average ride duration by rider type:

![average_ride_duration_by_rider_type](https://github.com/djr111/-Cyclistic---bike-share-project/assets/58305266/91374e8b-1c7d-4f3c-b498-1872a1921397)

Average ride duration by rider type also available on Tableau public: [link](https://public.tableau.com/app/profile/raimonds.buls/viz/Averageridelengthofcasualsvsmembers/Sheet1#1.)



Key findings:

As a data analyst, upon examining the Cyclistic bike trip data, it becomes evident that annual members exhibit a substantially higher frequency of bike usage compared to casual riders. Specifically, the data reveals that annual members utilize Cyclistic bikes with remarkable frequency, significantly surpassing the usage rates observed among casual riders. This trend underscores the distinct usage patterns between these two customer segments.

Furthermore, while annual members demonstrate a propensity for more frequent bike trips, their trip durations tend to be notably shorter compared to casual riders. This finding suggests that although annual members utilize Cyclistic bikes more often, their individual trips are characterized by shorter durations. Conversely, casual riders exhibit a contrasting behavior, as they engage in bike rides for significantly longer periods of time.

This analysis sheds light on the differing behaviors and preferences of Cyclistic's customer segments. The data suggests that while annual members prioritize frequent and shorter bike trips, casual riders are inclined towards fewer but longer-duration rides. Understanding these nuanced usage patterns is crucial for informing targeted marketing strategies aimed at maximizing annual memberships and optimizing the overall customer experience within the Cyclistic bike-share program.



![image](https://github.com/djr111/-Cyclistic---bike-share-project/assets/58305266/77d5f620-c442-4289-9704-3c4e56f42ad8)

(Reminder of business task: The goal is to maximize the number of annual memberships, as it has been identified that annual members are much more profitable for Cyclistic compared to casual riders.)

Recommendations based on analysis for marketing department:

1: Tailored Membership Packages:
   Develop customized membership packages that cater to the distinct preferences and usage patterns of both annual members and casual riders. Offer flexible subscription options, such as tiered membership levels or pay-as-you-go plans, to accommodate varying ride frequencies and trip durations. Highlight the benefits of annual memberships, such as discounted rates    or exclusive perks, to incentivize casual riders to transition into long-term subscribers.

2: Personalized Promotional Campaigns:
   Leverage customer segmentation and behavioral data to create personalized marketing campaigns targeted towards different customer segments. Utilize email marketing, social media advertising, and targeted promotions to communicate relevant offers and incentives to both annual members and casual riders. Tailor messaging and promotions based on ride frequency,        trip duration, and preferred bike types to enhance engagement and drive conversions.

3: Enhanced User Experience:
   Enhance the Cyclistic user experience by optimizing the bike-sharing platform and mobile app to better meet the needs of both annual members and casual riders. Implement features such as real-time ride tracking, trip planning tools, and in-app rewards programs to incentivize frequent usage and foster customer loyalty. Streamline the rental process and improve      bike availability and accessibility across docking stations to ensure a seamless and convenient experience for all users.

4: Educational Content and Resources:
   Develop educational content and resources to inform customers about the benefits of bike sharing and promote healthy and sustainable transportation options. Create blog posts, videos, and interactive guides that highlight the environmental, health, and economic advantages of cycling. Provide tips on bike safety, route planning, and bike maintenance to empower      users and encourage them to incorporate cycling into their daily routines.

5: Community Engagement Initiatives:
   Foster a sense of community and belonging among Cyclistic users by organizing community events, group rides, and social gatherings. Collaborate with local organizations, businesses, and advocacy groups to promote cycling culture and encourage participation in cycling-related activities. Sponsor local events, charity rides, and cycling competitions to raise         brand awareness and demonstrate Cyclistic's commitment to supporting active and sustainable lifestyles.



