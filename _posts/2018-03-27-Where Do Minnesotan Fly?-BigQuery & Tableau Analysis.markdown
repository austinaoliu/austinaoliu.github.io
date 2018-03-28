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

![Tableau Loading](https://github.com/aoliu95/aoliu95.github.io/raw/master/assets/images/tableau_loading.png)
<center>***Got GBs of data? Tired of waiting for Tableau's response?***</center>

You can save **70%** of your waiting time utlizing the power of **Cloud**! In this post, I'll show you how I used Google's Big Data platform "BigQuery" together with Tableau for Data Analysis and Visualization. 

###**Here is the [Tableau Dashboard](https://public.tableau.com/views/sun_2/Dashboard1?:embed=y&:display_count=yes&publish=yes)**

##What is BigQuery? 
BigQuery is Google's solution for Big Data Analysis. Compared with Hadoop, BigQuery can do better in real-time querying and data analysis. For other competitors like Apache Spark, Google's Bigquery offers easier setup and more flexible billing plan. Also, embedded with Google's IAM system, access control would be much easier compared with Apache's ZooKeeper. 
##Data Source
The data is from Minnesota local airline travel records of 2013 and 2014, in CSV format with 800+ MB size.
Data should first be uploaded onto Google Cloud Storge, or other Storge Service like S3. After that, heads to the Bigquery Control Pannel, and adds the file as your data source. Bigquery would automatically try to detect the schema. But you can also define it by yourself.

<center><img src="https://github.com/aoliu95/aoliu95.github.io/raw/master/assets/images/Schma.png" alt="Drawing" style="width: 300px;"/> </center> 

After adding the data to your BigQuery Data source, you can either wrote SQL queries through BigQuery's platform or connect your Tableau to Bigquery by authenticating throught the start page.
##Why BigQuery+Tableau

<center><img src="https://github.com/aoliu95/aoliu95.github.io/raw/master/assets/images/loading.png" alt="Drawing" style="width: 40px;"/></center>
<center>*We all see this icon pretty often.*</center>

We all know Tableau is not very good at working with huge dataset, especially calculations. Now with Bigquery, Tableau would send the calculation request in SQL query to the cloud and get result instantly. I tried myself and it cuts my waiting time from 10+ seconds to **less than** 1 second. Bigquery also enables people to share the same dataset without actully owning the data. So that your workbook could be live and mobile.

##What do we learn about Minnesotan's data


 


