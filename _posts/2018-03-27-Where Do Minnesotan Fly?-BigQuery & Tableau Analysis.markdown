---
title: "Where did Minnesotans Fly?-Flight Data Visualization"
layout: post
date: 2018-03-27 23:19
headerImage: true
blog: true
star: true
author: Ao Liu
description: See the trend behind billion rows of Airline Travel Records  
---

<center><img src="https://github.com/aoliu95/aoliu95.github.io/raw/master/assets/images/tableau_loading.png" style="width: 350px;"/> </center> 
<center>Got GBs of data? Tired of waiting for Tableau's response?</center>

You can save **70%** of your waiting time utlizing the power of **Cloud**! In this post, I'll show you how I used Google's Big Data platform "BigQuery" together with Tableau for Data Analysis and Visualization. 

### **Here is the [Tableau Dashboard](https://public.tableau.com/views/sun_2/Dashboard1?:embed=y&:display_count=yes&publish=yes)**

## What is BigQuery? 
BigQuery is Google's solution for Big Data Analysis. Compared with Hadoop, BigQuery can do better in real-time querying and data analysis. For other competitors like Apache Spark, Google's Bigquery offers easier setup and more flexible billing plan. Also, embedded with Google's IAM system, access control would be much easier compared with Apache's ZooKeeper. 
## Data Source
The data is from Minnesota local airline travel records of 2013 and 2014, in CSV format with 800+ MB size.
Data should first be uploaded onto Google Cloud Storge, or other Storge Service like S3. After that, heads to the Bigquery Control Pannel, and adds the file as your data source. Bigquery would automatically try to detect the schema. But you can also define it by yourself.

<center><img src="https://github.com/aoliu95/aoliu95.github.io/raw/master/assets/images/Schma.png" alt="Drawing" style="width: 300px;"/> </center> 

After adding the data to your BigQuery Data source, you can either wrote SQL queries through BigQuery's platform or connect your Tableau to Bigquery by authenticating throught the start page.
## Why BigQuery+Tableau

<center><img src="https://github.com/aoliu95/aoliu95.github.io/raw/master/assets/images/loading.png" alt="Drawing" style="width: 40px;"/></center>
<center>We all see this icon pretty often.</center>

We all know Tableau is not very good at working with huge dataset, especially calculations. Now with Bigquery, Tableau would send the calculation request in SQL query to the cloud and get result instantly. I tried myself and it cuts my waiting time from 10+ seconds to **less than** 1 second. Bigquery also enables people to share the same dataset without actully owning the data. So that your workbook could be live and mobile.

## What do we learn about Minnesotan's data
### 1.Time 
Minnesota people fly for different purposes on different seasons. During winter, people fly more for vacations and "warmer places", including **Las Vagas, Orlando or Cancun** (Especially during the days when temerature drops below 0). For other seasons, customers fly mainly for business purposes. Destinations includes San Francisco, Los Angeles and New York. 
###2. Advanced Booking
It follows the similar trend with the purposes. For vocational travel, people tend to plan **well ahead**. You could even see people book over **3** months ahead for a trip to Orlando. For businss trip, there would be **less planning** for ticket booking.
###3. Booking Source
**Outside booking** took over 40% of all the bookings. But we also noticed that, for vacational travels, customers also utlize "**Airline Vacation Bundle**" and "**Reservations**" more. Because a large porpotion of these customer are older generations. For business travel, we would see more in "Airline Website", as the average age for customers are younger.
###4.Airline Membership
For different destinations, the proportion of Airline Membership among  passengers are also different. People who fly for **business travel** are more likely to become member of the Airline Club, as we see higher membership percentage for SFO, LAX and DFW. 
###5.Premiums for the Airline
We would define the premium as the difference between ticket base price and what the passenger actual paid, which includes luggage fee, onboard purchase, taxes and other services. It's not surprising to see '**Vacation Package**' and '**Reservation**' offers good premium for the Airline. But we also saw "**Airline Website**" offers up-to-average premium. For Outside booking, the premium would be less than average. Flight to Cacun also offers higher premium, compared with other Business travels.
## Business Recommendations
1.Targetive Marketing Plan

2.Adjust price policy

3.Promote its own booking system



 


