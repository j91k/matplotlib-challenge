# MATPLOTLIB PROJECT

## Overview
This project utilized Matplotlib, Pandas, Scipy, and Sklearn to analyze and report the performances of Pymaceuticals' drug, Capomulin, against the other treatments regimes, highlighting key metrics such as tumor size reducation. The data was gathered from the most recent animal study involving 249 mice with SCC tumors. Observation and measurement of the tumor development were conducted over the course of 45 days. 
The analysis includes summaries and data visualizations using tables and charts.

### Key Componenets of the Report
1. **Data Preparation**
   - The mouse_metadata and study_results DataFrames are merged into a single DataFrame.
   - A cleaned DataFrame is done on the unique mice IDs by removing any mouse ID with duplicated time points.
   
2. **Statistics Summary**
   - A DataFrame is created to include an indexed column of each drug regimen.
   - Calculation based on tumor volume: mean, median, variance, standard deviation, and SEM.
   
3. **Data Visualization**
    - Bar Charts
       - To show the total number of rows(Mouse ID/Timepoints) for each drug regimen throughout the study with Pandas DataFrame.plot() and Matplotlib pyplot methods
       
    - Pie Charts
        - To show the distribution of female versus male mice using Pandas DataFrame.plot() and Matplotlib pyplot methods
       
    - Box Plot
       - To show the distribution of the final tumor volume for all the mice in each treatment group and any potential outliers are hightlighted.
       - The quartiles and IQR are calculated after final tumor volume of each mouse was gathered across four most promising treatment regimes: Capomulin, Ramicane, Infubinol, and Ceftamin. 
       - Determine any potential outliers by using the upper and lower bounds.
       
    - Line Plot
       - To show the line visualization of tumor volume versus time point for a single mouse that was treated with Capomulin.

    - Scatter Plot
       - To show the distribution of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

    - Linear Regression Model
       - To show the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatement regimen.
