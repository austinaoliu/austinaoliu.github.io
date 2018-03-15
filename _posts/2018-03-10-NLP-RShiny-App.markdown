---
title: "R Shiny App:NLP Next Word Prediction"
layout: post
date: 2018-03-15 01:19
headerImage: false
blog: true
star: false
author: Ao Liu
description: How can Natural Language Processing predict your next word
---
# 1.Data Processing
* First, all non-English characters are removed; numbers, punctuation, whitespace was also removed. All text is also changed to lowercase.
* Profane words are also removed. The project used Carnegie Mellon University's resource: [Offensive/Profane Word List.](https://www.cs.cmu.edu/~biglou/resources/bad-words.txt)
# 2.Prediction Algorithm
* Tokenization: used for finding the frequency of five types of n-gram: unigrams (single words), bigrams (two word phrases), trigrams (three words), quadgrams (four word) and quintgrams (five words).
* N-grams: indicate which words appear together in the text. (The higher the frequency of a certain n-gram, the more likely it is to be found in the corpus.)
* The predictive algorithm uses the n-gram frequency to suggest/ predict the next word based on the users input. The model checks the phrase length and starts with the quintgram, then moves onto the quadgram and so on. The model is a version of a 'back-off' [model](https://en.wikipedia.org/wiki/Katz%27s_back-off_model).
# 3.Actual R-shiny App
This is the [R-Shiny app](https://austin-liu.shinyapps.io/NLPNextWordPredicition/) based on N-gram Human Language Processing.![Test Image](https://github.com/aoliu95/aoliu95.github.io/raw/master/assets/images/NLP.png)



