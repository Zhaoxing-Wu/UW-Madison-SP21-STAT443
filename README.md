# UW-Madison SP21 STAT443 Classification and Regression Trees
Course repository own by Zhaoxing (Bella) Wu

Professor Name: Wei-Yin Loh

## Files
  - `lecture_note.pdf`: contains all lecture notes in SP21
  - `./homework/`: contains all 6 homeworks
  - `./final_project/`: contains the final project report and data source

## Final Project
### Project Name
Different Methods of Predicting the Mean of Individual Interests, Dividend, and Rental Income

### Abstract 
The purpose of this study is to compare and contrast the results of using different trees, forests, or logistic regression to estimate the mean of individual interests, dividend, and rental income with sampling weight. With different classification and regression methods, either the probability of response or the missing value for the variable of interest could be predicted for the estimation of the mean. The result of the study shows that GUIDE (Generalized, Unbiased, Interaction Detection and Estimation) classification forest and GUIDE regression stepwise linear tree give the best estimate among all other methods.

### Introduction
Nowadays, the majority of people choose to build wealth by investing in stocks, bonds or real estate to ensure consistent returns. Therefore, increasingly more people choose to make earnings not only from regular wages, but also from individual interests, dividend, and rental income as well. With the purpose of analyzing citizens’ financial situation, it would be worthwhile to estimate the personal interests, dividend, and rental income, while American Community Survey (ACS) provides a way of doing this. ACS collects Public Use Microdata Sample (PUMS) every year, which includes both person record and household record. In the person record, each observation represents a single person and the variable of interest INTP (the interest, dividend, and net rental income of each person in the past 12 months) is also collected. In this study, the dataset of the person record with 56670 observations and 288 variables is analyzed from the state of Minnesota, which has a population of 5.64 million by the year of 2019, ranked 22 in the United States. The aim of the paper is to apply different methods in predicting the mean of INTP with the sampling weight using the ACS PUMS dataset of
Minnesota.

### Model
  - GUIDE tree (default univ. splits/2nd best univ. split at root node, constant/stepwise)
  - GUIDE forest
  - RPART (classification/regression tree)
  - CTREE (classification/regression tree)
  - Random Forest
  - CFOREST
  - Logistic Regression

### R packages
`haven, sas7bdat, tidyverse, rpart, rpart.plot, party, Amelia, MASS, nnet, mice, randomForest, popbio`

### Results
<p align="left">
  <img src="https://github.com/zwu363/UW-Madison-SP21-STAT443/blob/main/final_project/figure/Picture1.png" width="350"
</p>
  
Figure 1: GUIDE Importance Score of Least Squared Regression Tree

<p align="left">
  <img src="https://github.com/zwu363/UW-Madison-SP21-STAT443/blob/main/final_project/figure/Picture2.png" width="350"
</p>
  
Figure 2: GUIDE Importance Score of Classification Tress

<p align="left">
  <img src="https://github.com/zwu363/UW-Madison-SP21-STAT443/blob/main/final_project/figure/Picture3.png" width="700"
</p>
  
Figure 3: the classification trees build by GUIDE

<p align="left">
  <img src="https://github.com/zwu363/UW-Madison-SP21-STAT443/blob/main/final_project/figure/Picture4.png" width="700"
</p>
  
Figure 4: the classification trees built by GUIDE, with INTP excluded

<p align="left">
  <img src="https://github.com/zwu363/UW-Madison-SP21-STAT443/blob/main/final_project/figure/Picture5.png" width="700"
</p>
  
Figure 5: The classification tree and regression tree built by RPART

<p align="left">
  <img src="https://github.com/zwu363/UW-Madison-SP21-STAT443/blob/main/final_project/figure/Picture6.png" width="400"
</p>
  
Figure 6: Plots of observed versus fitted values for different classification methods

<p align="left">
  <img src="https://github.com/zwu363/UW-Madison-SP21-STAT443/blob/main/final_project/figure/Picture7.png" width="700"
</p>
  
Figure 7: the regression trees built by GUIDE

<p align="left">
  <img src="https://github.com/zwu363/UW-Madison-SP21-STAT443/blob/main/final_project/figure/Picture8.png" width="400"
</p>
  
Figure 8: Plots of observed versus fitted values for different regression methods
