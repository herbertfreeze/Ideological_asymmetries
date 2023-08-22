# Ideological Asymmetries on Twitter 


## Overview
This respository contains the analysis code for "Liberals Engage With More Diverse 
Policy Topics and Toxic Content Than Conservatives on Social Media" (https://osf.io/x59qt/). 

## Datasets

There are two main datasets: master_df.csv contains the supply-side data, which are congressional tweets
from between 2009 and 2019. It includes metadata like Congressperson position, LIWC Scores,
incivility, weighted ideological score, and the in-/out-group category.
master_RT_df.csv contains the demand-side data, which consists of retweet events from users, along with metadata associated with the tweet and the retweeter (user).

The original dataset is based on [Frimer et al. 2022.](https://journals.sagepub.com/doi/abs/10.1177/19485506221083811). The topics2labels.csv contains the [Comparative Agenda Project Policy Issue labels](https://comparativeagendas.s3.amazonaws.com/codebookfiles/Codebook_PAP_2019.pdf).

## Notebooks

There are three notebooks. Main figures produce the cross-sectional analyses. Topic entropy contains the entropy computations for the demand-side: user-level aggregations of diversity. Catboost Regression contains the gradient-boosting regression and Shapley value analysis for the gradient-boosting trees.

## Dependencies

```
numpy
pandas
seaborn
CatBoost
matplotlib
Scipy
sklearn
```
## System Requirements & Installation
The code has been tested using Anaconda on the following operating systems:
```
Ubuntu 20.04
macOS: Monterey
Windows 10
```
Installation time depends on hardware but is the same as the standard Anaconda installation.

