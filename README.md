# CF-Democracy-Happiness
 Data Analysis: Does Democracy Make People Happy?

* [**Link to Tableau-Storyboard**](https://public.tableau.com/views/DoesDemocracyMakePeopleHappy2025-02-17V01/DemocracyandHappiness?:language=en-GB&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Overview

Extremist parties have gained political influence in many countries over the last years.
One of the frequently mentioned explanations for this is, that people are unhappy with how democracy works and frustrated by the increased costs of living. The Covid-19 measures, which limited personal freedoms in many countries, are also frequently mentioned as contributing factors. 
While voters' decisions are influenced by many factors, this project looks specifically at: 

* Are people in more democratic societies happier? 
* Does inflation have a significant impact on happiness? 
* Have more stringent COVID-measures led to a decline in happiness? 

## Project Structure

The analysis is divided into nine Jupyter notebooks, each focusing on different aspects of the data:
1. Descriptive Analysis and Data Exploration of World Happiness, Inflation and Democracy-Data
1.1. Data Merging
2. Exploring Relationships
3. Geographical Analysis
4. Machine Learning: Regression
5. Machine Learning: Clustering
6. Time Series Analysis
7. Data Preparation and Merge of Covid-Stringency-Data
8. Machine Learning: Regression of Covid-Stringency Data

## Data Sources
**World Happiness Report 2024**: Yearly report that calculates happiness per country in up to 137 countries based on six key variables. Higher happiness-scores (range: 1-10) are better. The report was first released in 2005 with data from only 25 countries. This analysis used data as of 2008 when 110 countries were captured by the report. [Source](https://worldhappiness.report/data/) 

**Global Inflation Data**: World Bank data on inflation in 267 countries [Source](https://databank.worldbank.org/source/world-development-indicators) 

**Democracy Index**: Measurement of the quality of democracies in 167 countries since 2006. Higher values (0-10) indicate more democratic regimes. The index is compiled by the Economist Intelligence Unit ([Source](https://ourworldindata.org/grapher/democracy-index-eiu) 

**Covid-19 Stringency Index**: Measurement of the stringency of COVID-19 measures, created by the Blavatnik School of Government at University of Oxford between 2020 and 2024. The index is based on factors such as travel bans, school closures, etc. [Source](https://ourworldindata.org/metrics-explained-covid19-stringency-index) 
  
## Limitations 
* The number of countries covered by the datasets changes over time. 
* Some datasets are lacking data for some countries and/or years. In the case of democracy values, the data was imputed from previous/following years. However missing inflation data was not imputed and remained missing. 
* The Democracy Index and the World Happiness Report are based on surveys and might contain different forms of bias. However, given that both surveys are conducted by renowned expert organisations, this concern is minimal. 
* Additional limitations and assumptions can be found in the respective codebooks and annexes. 

## Key Findings

The data suggest that **people living in more democratic societies are generally happier than those living in more autocratic societies** (correlation: 0.61). However, that is not always the case and other factors such as GDP (correlation: 0.78), social support (correlation: 0.72) or life expectancy (correlation: 0.72) have a larger impact. 

The data further suggests that **inflation has only an extremely limited impact on happiness** (correlation: -0.2). This is surprising since media reports in the last few years suggested strongly that inflation was one of the main drivers of unhappiness, leading to an increase in authoritarianism. The data analysed here does not support that assumption. 

Similarly, there is **no indication that more intense Covid-19 restrictions led to more unhappiness** compared to less restrictive countries. 

Overall, this analysis has shown that **supporting authoritarian-leaning political actors is contrary to the interests of people who expect to live happier lives.** 

## Possible Next Steps
Happiness depends on many factors, many of which are already taken into account in the World Happiness Report. Additional factors to look into could be:
* Correlations between economic factors and support for extremist parties, rather than regime types. 
* Correlations between income inequality, happiness and regime type. 

## Methodology

**Exploratory Data Analysis**
* Data cleaning and preprocessing
* Visualization of key features and relationships

**Statistical Analysis**
* Correlation analysis
* Linear regression
* Clustering analysis

**Geographical Analysis**
* Choropleth mapping of happiness data

**Time Series Analysis**
* Decomposition of time series data
* Stationarity testing (Dickey-Fuller Test)

**Key Visualizations**
* Correlation matrices and heat maps
* Scatterplots and pair plots
* Choropleth maps
* Clustering visualizations

## Tools and Technologies Used
* Excel
* Python
* Jupyter Lab
* Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels
* Tableau Public (for visualization)

## How to Use This Repository
1. Clone the repository
2. Install required libraries
3. Open the Jupyter notebooks in order, starting with "1 Descriptive Analysis and Exploration.ipynb"

### Author
Timo Lüge