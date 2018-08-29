# [Modeling structured population dynamics using data from unmarked individuals](https://onlinelibrary.wiley.com/doi/full/10.1890/13-1131.1)

### Elise F. Zipkin, James T. Thorson, Kevin See, Heather J. Lynch, Evan H. Campbell Grant, Yoichiro Kanno, Richard B. Chandler, Benjamin H. Letcher, J. Andrew Royle

### Ecology

### Please contact the first author for questions about the code or data: Elise F. Zipkin (ezipkin@msu.edu)
________________________________________________________________________________________________________________________________________

## Abstract
The study of population dynamics requires unbiased, precise estimates of abundance and vital rates that account for the demographic structure inherent in all wildlife and plant populations. Traditionally, these estimates have only been available through approaches that rely on intensive mark–recapture data. We extended recently developed N-mixture models to demonstrate how demographic parameters and abundance can be estimated for structured populations using only stage-structured count data. Our modeling framework can be used to make reliable inferences on abundance as well as recruitment, immigration, stage-specific survival, and detection rates during sampling. We present a range of simulations to illustrate the data requirements, including the number of years and locations necessary for accurate and precise parameter estimates. We apply our modeling framework to a population of northern dusky salamanders (Desmognathus fuscus) in the mid-Atlantic region (USA) and find that the population is unexpectedly declining. Our approach represents a valuable advance in the estimation of population dynamics using multistate data from unmarked individuals and should additionally be useful in the development of integrated models that combine data from intensive (e.g., mark–recapture) and extensive (e.g., counts) data sources.


## **Data**

[saldata.aggregated_A.csv](https://github.com/zipkinlab/Zipkin_etal_2014_Ecol/blob/master/saldata.aggregated_A.csv) - Adult salamander counts for 21 sites from 2005-2011, with two sampling events per year
[saldata.aggregated_J.csv](https://github.com/zipkinlab/Zipkin_etal_2014_Ecol/blob/master/saldata.aggregated_J.csv) - Juvenile salamander counts for 21 sites from 2005-2011, with two sampling events per year

## **Code**

[Wrapper R code_salamander application.R](https://github.com/zipkinlab/Zipkin_etal_2014_Ecol/blob/master/Wrapper%20R%20code_salamander%20application.R) - Start with this file. This code reads and formats the data and then fits a structured Dail-Madsen model using the associated JAGS code "[JAGS code_salamander application.R](https://github.com/zipkinlab/Zipkin_etal_2014_Ecol/blob/master/JAGS%20code_salamander%20application.R)". The code produces a summary of the parameter estimates for the model and model diagnostics (e.g., traceplots and R-hat statisic).

[salamander_leslie matrix.R](https://github.com/zipkinlab/Zipkin_etal_2014_Ecol/blob/master/salamander_leslie%20matrix.R)" - estimates the population growth rate, lambda, using the full posterior distribution.
