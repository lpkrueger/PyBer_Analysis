# PyBer_Analysis
Module 5, Python & Pandas - UNCCH Data Analytics Bootcamp, Spring 2023


## Project Overview
    ### Overview of the analysis: Explain the purpose of the new analysis.

### Purpose
As a data analyst at PyBer, I've been assigned to perform analysis on rideshare data spanning from January to late April of 2019, using large CSV files as the data source. The desired outcome is visualization of ridesharing data by city type to inform decision-makers at PyBer whose aim is to improve rideshare affordability and access in underserved neighborhoods. 

## Method
 Using Python Pandas and Matplotlib libraries in the Jupyter Notebook environment, I imported the raw source files and created a summary DataFrame and a multiple-line graph that depict the total weekly fares for each city type. 

Sample of code used to format colums of "pyber_summary_df" summary DataFrame (image belwo). 
```
    format_dict = {'Total Rides':'{0:,.0f}',
              'Total Drivers':'{0:,.0f}',
              'Total Fares':'${0:,.2f}',
              'Average Fare per Ride':'${0:,.2f}',
              'Average Fare per Driver':'${0:,.2f}'}
    pyber_summary_df = pyber_summary_df.style.format(format_dict)
    pyber_summary_df
```
## Resources
- Data Sources:
    [city_data]](/main/Resources/city_data.csv)
    [ride_data]](/main/Resources/ride_data.csv)
- Software: Python 3.10.5
- IDE: Jupyter Notebooks

## Results
Ridesharing summary DataFrame by city type:
    ![pyber_symmary_df](/main/analysis/pyber_symmary_df.png)

Ridesharing weekly fares DataFrame by city type:
    ![weekly_fares_df](/main/analysis/weekly_fares_df.png)

A multiple-line chart of total fares for each city type:
    ![PyBer_fare_summary](/main/analysis/PyBer_fare_summary.png)

Jupyter Notebook file containing all data analysis source code:
    [PyBer_Challenge]](/main/PyBer_Challenge.ipynb)

## Summary
Drivers in urban cities don't make much money in fares - less than half that of suburban drivers and roughly one quarter of rural drivers. Also the average fare per ride is $10 more in rural than urban cities. It might be a good idea to increase fares in urban cities to boost the driver compensation. Also, recruiting more drivers in rural areas could reduce the fares for rural riders, which may offer more access and affordability to them for ridesharing. Both the rural and suburban ridesharing fares seem more stable (flat) over time than the urban fares. This may be attributable to the difference in scale. 
 