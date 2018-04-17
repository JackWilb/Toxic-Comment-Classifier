Natural Language Processing In R: A Wikipedia Case Study
========================================================
author: Jack Wilburn and Rob Squire
font-family: Georgia
date: 20th April 2018
autosize: true

Motivation
========================================================

* Kaggle
  - $50,000
* Skills
  - New
  - Old

Objectives
========================================================

* NLP
  - Body Of Text
  - Useful Variables
  - Example
* Predictive Modeling
  - Explantory Variables
  - Response Variable

Exploratory Data Analysis
========================================================


```
[1] "Explanation\nWhy the edits made under my username Hardcore Metallica Fan were reverted? They weren't vandalisms, just closure on some GAs after I voted at New York Dolls FAC. And please don't remove the template from the talk page since I'm retired now.89.205.38.27"
[2] "D'aww! He matches this background colour I'm seemingly stuck with. Thanks.  (talk) 21:51, January 11, 2016 (UTC)"                                                                                                                                                         
```

```
[1] "id"            "comment_text"  "toxic"         "severe_toxic" 
[5] "obscene"       "threat"        "insult"        "identity_hate"
```

Structure
========================================================


```
# A tibble: 1 x 8
  id     comment_text             toxic severe_toxic obscene threat insult
  <chr>  <chr>                    <int>        <int>   <int>  <int>  <int>
1 00009… "Explanation\nWhy the e…     0            0       0      0      0
# ... with 1 more variable: identity_hate <int>
```




Data Exploration
========================================================
##Libraries

```r
library(readr)
library(stringi)
library(quanteda)
library(dplyr)
library(caret)
library(glmnet)
library(doParallel)
library(tidytext)
library(data.table)
library(sentimentr)
```

##Exploratory
Now that we have some additional variables lets explore the data a bit.  
First lets count what we have.








```
Error in UseMethod("tbl_vars") : 
  no applicable method for 'tbl_vars' applied to an object of class "c('integer', 'numeric')"
```
