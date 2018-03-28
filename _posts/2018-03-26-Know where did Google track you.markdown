---
title: "Know where has Google tracked you - Location History Visualization App"
layout: post
date: 2018-03-26 21:35
headerImage: true
blog: true
star: true
author: Ao Liu
description: See how much these giant companies have known about you
---

After the scandal of [Cambridge Analytica](https://www.nytimes.com/2018/03/19/technology/facebook-cambridge-analytica-explained.html), I start to wonder: How much have these Internet companies known about me? 

There are some methods you can find some of the data they have collected, including [Google Takeout](https://takeout.google.com/) and [Facebook](https://www.facebook.com/help/302796099745838). Some people already find it surprising that Facebook even recorded your [call list](https://abcnews.go.com/Technology/download-call-list-facebook-access/story?id=54053309). 

<img src="https://github.com/aoliu95/aoliu95.github.io/raw/master/assets/images/loc.jpg" width="40%">

One of the most sensitive data is the location history. Basically they know every place you have been, and even the speed you moved sometimes. So I wrote a small Shiny App to visualize your Google Location History. Although I know that, due to being an Android User for two years, Google may collected some thing *interesting*. But I don't expect to be that much! My dorm, my home, even the spot I hanged out with someone! 

![My Loc History](https://github.com/aoliu95/aoliu95.github.io/raw/master/assets/images/Example.gif)
*Wow, you really know me a lot Mr.Google.*

If you want to try out and be surprised. [Here is the app](https://austin-liu.shinyapps.io/google_location_privacy_app/).

`Privacy: We are not going to be another Cambridge Analytica! Your data would be uploaded to RShiny's cache. It will only be used for the purpose of rendering this visualisation. ANY FILE would be permently wiped once you closed the app. You are also welcomed to audit the code at` [A Light Data Lab Github Page](https://github.com/aoliu95/google_location_privacy_app)

