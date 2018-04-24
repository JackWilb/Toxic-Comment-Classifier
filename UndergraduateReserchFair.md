Natural Language Processing In R: A Wikipedia Case Study
========================================================
author: Jack Wilburn and Rob Squire
font-family: Georgia
date: 20th April 2018
autosize: true



Motivation
========================================================

* Text Analysis
* Develop Techniques
  - Data Aggregation/Cleaning
  - Modeling
  - Reporting

Objectives
========================================================

* Natural Language Processing (NLP)
  - Body Of Text
  - Useful Variables
  
* Predictive Modeling
  - Explantory Variables
  - 6 Response Variables
  - Inference
  
Methods 
========================================================

* Explore Raw Data

* Clean Data

* Create Variables

* Split data
  - Training/Test
  
Methods 
========================================================  

* Implement models 
  - Cross Validated Logistic Regression

* Assess Accuracy
  - Confusion Matrix

Libraries
========================================================



* readr
* stringi
* quanteda
* dplyr
* caret

***

* glmnet
* doParallel
* tidytext
* data.table
* sentimentr

Exploratory Data Analysis
========================================================



* Structure Of The Data

```
                id
1 003dbd1b9b354c1f
                                                                                                                                                                                                                                                              comment_text
1 You can do all you're doing right now but if you get a username you'll be able to do more and have more impact is what I'm saying. And you seem to be very familiar with everything so you probably have a username? Just get one, it takes 10 seconds.  (talk•contribs)
  toxic severe_toxic obscene threat insult identity_hate
1     0            0       0      0      0             0
```

Exploratory Data Analysis
========================================================



* Prevalence

  * Toxic: 9.5844483 %.
  
  * Severe_toxic: 0.9995551 %.
  
  * Obscene: 5.2948217 %.
  
  * Threat: 0.2995532 %.
  
  * Insult: 4.9363606 %.
  
  * Identity Hate: 0.8804858 %.

Tidy Text Word Analysis
========================================================
















```
Error in parse(text = x, srcfile = src) : <text>:3:1: unexpected input
2:     ggplot(aes(x = reorder(term, freq), y = freq)) +
3: <<
   ^
```
