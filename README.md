# Mixture Conditional Regression with Ultrahigh Dimensional Text  Data for Estimating Extralegal Factor Effects

This repository provides python codes for the mixture conditional regression (MCR) with ultrahigh dimensional text  data accompanying the paper.

> Shi, J., Wang, F., Gao, Y., Song, X., and Wang, H. (2023). Mixture Conditional Regression with Ultrahigh Dimensional Text Data for Estimating Extralegal Factor Effects. arXiv preprint arXiv:2311.07906.

## Overview

The repository consists of two parts: one is the code for simulation studies, and the other is that for real data.

## PART 1. Simulation

- The following code files can be used to reproduce simulation results presented in the main paper.

|File name| Description |
|-------------|---------------|
|**`Initial_Estimator.ipynb`**| Jupyter notebook to implement the initial estimation. |
|**`Response_Probability.ipynb`**| Jupyter notebook to implement the response probability estimation. |
|**`Membership_Estimator.ipynb`**| Jupyter notebook to implement the class membership identification. |
|**`Final_Estimator.ipynb`**| Jupyter notebook to implement the updated final estimation. |
|**`BIC_select_K.ipynb`**| Jupyter notebook to implement the BIC selection for the number of classes K. |
|**`Results_plot.ipynb`**| Jupyter notebook to visualizing the estimation results above. |


## PART 2. Real Data Analysis

### (1). Real data
The Chinese judgement data needed for reproducing the results is named as data_room.csv. 

- Brief description: This dataset was randomly sampled from the 2018 Chinese burglary judgements. Each row represents a sample of cases.
- Response variable: penalty_prison_length, continuous.
- Extralegal factors (interested variables): Columns 2 to 8, the defendant's demographic characteristics.
- Legal factors: Columns 9 to 6586 are all keyword variables, which are extracted from the criminal facts in judgements.

### (2). Code files and estimation results

|File name| Explanation |
|-------------|---------------|
|**`Real_data_BICselect_K.ipynb`**| Jupyter notebook to implement the BIC selection for the number of classes K in real data analysis. |
|**`Real_results.ipynb`**| Jupyter notebook to implement MCR method in real data and compares them with OLS method. |
|**`BIC_K_results.csv`**| BIC estimation results for K from 1 to 20.|
|**`XZ_select.csv`**| Selected control variables. |
|**`mcr_K7_B1000.csv`**| MCR estimation results. |
|**`ols_B1000.csv`**| OLR estimation results. |

