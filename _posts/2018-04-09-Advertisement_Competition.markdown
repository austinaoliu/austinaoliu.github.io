---
title: "Advertisement Competition between top 3 Fast Food Chains -Tableau Vizulization and Analysis"
layout: post
date: 2018-04-09 16:19
headerImage: true
blog: true
star: false
author: Ao Liu
description: See how fast food chains compete with each other on your screen
---

![](http://p6c7brrnk.bkt.gdipper.com/ham.png?imageMogr2/thumbnail/!70p)
 
Data visulizaiton would always be fun if you have some interesting data. For this one, I got this data from parts of the take home challenge. This is what I made in two hours. **Here is the [Tableau Dashboard](https://public.tableau.com/views/Fast_foodTVAd/Dashboard1?:embed=y&:display_count=yes&publish=yes)**.

![](https://github.com/aoliu95/aoliu95.github.io/raw/master/assets/images/tableauburger.gif)

## Data Introduction
According to [QSR 50](https://www.qsrmagazine.com/QSR-50) , **McDonald’s**, **Burger King** and **Wendy’s** are ranked as the top three fast food chains in the US.

### -Data Source:
Alphonso Airings Report for McDonald’s, Burger King and Wendy’s, collected between Jan 1st, 2018 and Apr 6th, 2018

### -Dimensions:

**Advertisement Content**: Title, Brand, Product, Category

**Network**: Network Name, Network Type, Show, Pod Position

**Time**: Date and time, Time Zone, length, EQ Units

## Exploratory Analysis - Content
**McDonald’s**:Aired on **62** Networks with **1,796** Shows

Most Aired Advertisement:
“McDonald‘s ”I’m Lovin‘ It“ TV Commercial” with **2,890** EQ units


**Burger King**: Aired on **89** Networks with **2,962** Shows

Most Aired Advertisement:
“Burger King Whopper And Crispy Chicken 2 For \$ 6 Mix Or Match Your Way“ TV Commercial” with **10,331** EQ units


**Wendy’s**: Aired on **70** Networks on **2,090** Shows

Most Aired Advertisement: 
Wendy‘s 4 For \$ 4 Quality Is Our Recipe TV Commercial with **5,037** EQ units

## Exploratory Analysis - Network

![](http://p6c7brrnk.bkt.gdipper.com/mc_net.png?imageMogr2/thumbnail/!70p)
![](http://p6c7brrnk.bkt.gdipper.com/bgnet.png?imageMogr2/thumbnail/!70p)
![](http://p6c7brrnk.bkt.gdipper.com/windynet.png?imageMogr2/thumbnail/!70p)

All three companies prefer putting their ad on **Sports Related Events**, especially for **Wendy’s**, who focuses more on Baseball and Basketball. 
McDonald’s and Burger King also put considerable resources on entertainment channels.

## Exploratory Analysis - Time
![](http://p6c7brrnk.bkt.gdipper.com/mctime.png?imageMogr2/thumbnail/!70p)
![](http://p6c7brrnk.bkt.gdipper.com/bgtime.png?imageMogr2/thumbnail/!70p)
![](http://p6c7brrnk.bkt.gdipper.com/wendytime.png?imageMogr2/thumbnail/!70p)

For the time of the day, **Wendy’s** focuses more on **Daytime part**, while Burger king puts their ads more evenly between **Prime Time** and **Daytime** for higher audience coverage.  Both three chains put more resources for **weekends**, but Burger King emphasis more on **Sundays**. 


## Competition Analysis
But how would they compete with each other on the **limited audience resources**?

#### Data Preparation
To compare the brand on the same level, we took only the networks with the top **7** viewers, including CBS, NBC, ABC, Fox, Univision, USA and ESPN.
#### Measurements:  

![](http://p6c7brrnk.bkt.gdipper.com/1525459603.png?imageMogr2/thumbnail/!70p)

### Competition Analysis – Across all channels

<center><img src="http://p6c7brrnk.bkt.gdipper.com/acrossch.png?imageMogr2/thumbnail/!70p" style="width: 550px;"/> </center>

#### Sports
![](http://p6c7brrnk.bkt.gdipper.com/1525459674.png?imageMogr2/thumbnail/!70p)
Sports Networks like ESPN is the main battle round for fast food chains, where Burger King takes higher voice during weekdays, but Wendy’s is bidding hard for weekend airing times, targeting Sports Live audiences

#### Network Preference
![](http://p6c7brrnk.bkt.gdipper.com/1525459701.png?imageMogr2/thumbnail/!70p)
McDonald’s takes dominance in national networks including NBC, ABC, CBS and Fox, for wider audience reach, while Burger King dominates USA Network. 

#### Weekend vs. Weekday
![](http://p6c7brrnk.bkt.gdipper.com/1525459717.png?imageMogr2/thumbnail/!70p)
For national networks, Wendy’s strategy is that it puts their most resources bidding for airing times for weekends, where there is higher possibilities that target audience would watch television. It even gives up some of the network for some day. 
We also saw some huge drops for McDonald's during weekends.

### Competition Analysis – Day Parts at ESPN & CBS

We would compare brands detailed airtime strategy between two different types of networks, we took ESPN and CBS as the example. 

#### ESPN ![](http://p6c7brrnk.bkt.gdipper.com/1525459770.png?imageMogr2/thumbnail/!70p)


<img src="http://p6c7brrnk.bkt.gdipper.com/espn.png?imageMogr2/thumbnail/!70p") style="width: 550px;"/>


Insight:

**Wendy‘s** loves weekends. It puts most their expense and took the dominance for **Day Time and Early Fringe** during weekends, where the weight could be as high as 76%. They also took much advantage of **Weekend Prime Time**.

**Burger King** bids more for **Over night and Early morning** for weekdays and weekends, while McDonald’s voice is weight is relatively **stable**.

#### CBS ![](http://p6c7brrnk.bkt.gdipper.com/1525459851.png?imageMogr2/thumbnail/!70p)


<img src="http://p6c7brrnk.bkt.gdipper.com/cbs.png?imageMogr2/thumbnail/!70p") style="width: 550px;"/>


Insight:

When it comes to non-sporting networks, **Wendy’s** weight is much lower, it gives up over 50% of the day parts, but still it invest money into Weekend Daytime, and took dominance at **Sunday on Early Fringe.**

**McDonald’s** takes the **absolute dominance** for most of the dayparts, except some of the **day time and overnight programs**, where Burger King takes the lead. 

## What could be done further?

![](http://p6c7brrnk.bkt.gdipper.com/1525459916.png?imageMogr2/thumbnail/!70p)
If given more data about the geographic information of audiences on the network and the show, and the cost of advertisement, we could conduct **cost analysis** and research on **optimizing the advertising strategy** for the brand, to achieve the best audience exposure given the least advertisement cost.

![](http://p6c7brrnk.bkt.gdipper.com/1525459928.png?imageMogr2/thumbnail/!70p)
Together with the watch preference data gather from online advertisement platform including Facebook and YouTube, we could adjust our television advertisement contents **dynamically** for the best result. 
