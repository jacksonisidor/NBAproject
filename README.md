# NBA Data Science Project

## Goal
The primary objectives of this data science project are:
- Predicting the next class of NBA Hall of Famers and assigning a percentage chance of making the Hall of Fame to each active player.
- Predicting NBA all-stars for a given year based on their season statistics. The model will be used in February 2024 to predict next season's all-stars.
- Clustering players into tiers based on career success (superstar down to bust).

I had a few inspirations when deciding on this project. The first comes from Basketball Reference - they have a page on their website titled "Hall of Fame Probability." I remember seeing this when I was younger and being so lost on how they could have managed to come up with these percentages. It opened my eyes to how powerful statistics can be. After studying data science myself, I connected the dots on how they must have created it and it drove me towards making my own up-to-date version with what I believe makes a Hall of Famer.

My inspiration for the all-star predictions mostly comes from the fan voting system. It causes problems every year and theres always intense debate on who got snubbed. In my opinion, it would be better if we could put bias aside and reward players based on statistical output. Hopefully, this model can do just that and be accurate enough to predict the all-stars of any season, potentially followed by was really snubbed each year. 

## Overview
This repository contains a comprehensive data science project that delves into the analysis of NBA data. The project encompasses various stages of the data science pipeline, including data preprocessing and cleaning using pandas, creating insightful visualizations using Tableau, and implementing advanced regression and machine learning models with scikit-learn.

## Data Sources
The original data files utilized in this project are sourced from Sumitro Datta's dataset on Kaggle. The 'preprocessing.ipynb' file contains the steps taken to preprocess and clean the data. The resulting CSV files, located in the 'Data' folder, are then employed for subsequent analysis and modeling.

## Project Structure
#### Data Folder
  - `preprocessing.ipynb`: A Jupyter Notebook outlining the meticulous data preprocessing and cleaning steps undertaken.
  - `careers.csv`: A dataset encompassing NBA players' career statistics.
  - `modern_seasons.csv`: A dataset containing NBA season statistics from the modern era.
  - `seasons.csv`: A dataset comprising NBA season statistics since 1947.
  - 'References.md': Credit to the sources I used to create the aformentioned datasets

#### visualization Folder:
  - `ASG_Factors.md`: Visualizations showcasing the relationship between season statistics and all-star selections.
  - `HOF_Factors.md`: Visualizations illustrating the link between career statistics and Hall of Fame status.

## Coming soon
I am actively working on the following components to provide a more comprehensive analysis:
- `Regression.ipynb`: A Jupyter Notebook focusing on in-depth regression analysis using scikit-learn.
- `Predictions.ipynb`: A Jupyter Notebook detailing machine learning predictive models using scikit-learn.
- `Clustering.ipynb`: A Jupyter Notebook covering machine learning clustering analysis with scikit-learn.

Stay tuned for more updates as I delve deeper into the exciting world of NBA data analysis


