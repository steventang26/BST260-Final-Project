# BST260-Final-Project

Harvard Chan School | 2021 Fall | BST260 Final Project (Group 12)

## Team Members 
The following students contributed to this project: 

1. Xiang Bai 
2. Jennifer Dai 
3. Justin Farmer
4. Yu Fu
5. Steven Tang 

## Project Title
Predict COVID-19 Mortality Risk using Environmental, Behavioral, and Socioeconomic Factors among the U.S. Population

## Background
In 2020, coronavirus disease 2019 (COVID-19) is attacking human beings in the global scope as the worst public health crisis in a century. Here in the United States, after more than a year of the devastation caused by the pandemic, researchers and local policymakers are still facing urgent public health questions to mitigate the disease’s burden on the population level. Within the focus on environmental risk factors, one of the significant public health approaches is to evaluate whether long-term exposure to air pollution may lead to a higher incidence of COVID-19 death outcomes among the U.S. population.

According to data from Johns Hopkins University, more than 353,000 coronavirus deaths have been reported this year. Many of the pre-existing conditions that increase the risk of COVID-19 mortality are the same diseases that are affected by long-term exposure to air pollution. Long-term exposure to PM2.5 has been connected to a number of comorbidities, including cardiovascular and lung disease, that have been linked to poor prognosis and death in COVID-19 patients. However, the majority of the studies focused on the association between PM2.5 and COVID-19 cases rather than COVID-19 mortality. Moreover, these studies only have data up to mid-June 2020, which was likely to be biased and of lower generalizability since they only included the first wave COVID-19 cases.

In this study, we directly investigated the impact of air pollution on COVID-19 mortality risk by leveraging cumulative COVID-19 mortality data in 3,093 counties across the U.S. nationwide, updated to 2021. 

## Objectives
1. To investigate the effect of long-term exposure to air pollution on COVID-19 outcomes
2. To use machine learning to predict the number of deaths COVID-19 deaths from 03/22/20 to 10/31/21
3. To understand if the trend in county-level COVID-19 deaths associated with long-term exposure to air pollution are the same before and after the introduction of vaccines

## Data Set Basics 
The dataset includes all continental U.S. counties which had reported at least one COVID-19 death and have valid monthly PM2.5 data from 2000-2018. Data sources are all publicly available (https://github.com/wxwx1993/PM_COVID). 

The county-level COVID-19 deaths count is extracted from Johns Hopkins University the Center for Systems Science and Engineering (JHU-CSSE) Coronavirus Resource Center (https://coronavirus.jhu.edu/). 

Averaged PM2.5 concentration across the period 2000-2018  was linked to each county by leveraging data from Atmospheric Composition Analysis Group (https://sites.wustl.edu/acag/).

## Design Overview
We will modify the code from the research team github to extract the relevant data from JHU-CSSE through 10/31/2021. Data for the introduction of vaccines will be determined by a literature search. All data will be stored in a shared group Github. 

For this project we will use machine learning techniques to predict the number of COVID-19 deaths in a county from 03/22/2020 to 10/31/21.

We will then compare these numbers to the actual reported number of cases. We will perform the statistical analysis for the full data (through 10/31/21) to see if these models still describe the data into the late phase of the pandemic. Secondary explorations will include comparing the time frame up to the introduction of the vaccine to the time after the vaccine to see if these models fit the data for a population with available vaccines. To aid in this process, we will create maps of the US depicting county-level COVID-19 deaths, SES, PM.25. Finally, we will incorporate these maps into a SHINY app that allows for users to toggle between maps and look at individual counties.

## Reference
1. Wu, X., Nethery, R. C., Sabath, M. B., Braun, D. and Dominici, F., 2020. Air pollution and COVID-19 mortality in the United States: Strengths and limitations of an ecological regression analysis. Science advances, 6(45), p.eabd4049.

2. A pre-print version can be found at: Exposure to air pollution and COVID-19 mortality in the United States. Xiao Wu, Rachel C. Nethery, Benjamin M. Sabath, Danielle Braun, Francesca Dominici. medRxiv 2020.04.05.20054502; doi: https://doi.org/10.1101/2020.04.05.20054502
