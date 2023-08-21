# NBA Data Science Project

## Goal
The primary objectives of this data science project are:
- Predicting the next class of NBA Hall of Famers and assigning a percentage chance of making the Hall of Fame to each active player.
- Predicting NBA all-stars for a given year based on their season statistics. The model will be used in February 2024 to predict next season's all-stars.
- Clustering players into tiers based on career success (superstar down to bust).

My project draws inspiration from various sources, including Basketball Reference's 'Hall of Fame Probability' page, which left young-me intrigued by the power of statistics. After delving into data science myself, I discovered the methodologies behind such calculations, prompting me to create an updated and personalized version.

My inspiration for the all-star predictions comes from the perennial debate and controversy around the fan voting system. In response, I sought to create a predictive model that goes beyond biases and instead relies on statistical output to identify deserving All-Stars. By utilizing data-driven insights, I hope to offer an accurate prediction of each season's All-Star roster and shed light on potential snubs. 

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
  - `References.md`: Credit to the sources I used to create the aformentioned datasets

#### visualization Folder:
  - `ASG_Factors.md`: Visualizations showcasing the relationship between season statistics and all-star selections.
  - `HOF_Factors.md`: Visualizations illustrating the link between career statistics and Hall of Fame status.

#### Predictions Folder
  - `hof_model.ipynb`: A Jupyter Notebook containing the creation of the Hall of Fame predictive model
  - `hof_chances_list.csv`: A list of active players and their Hall of Fame probability assigned by the model
  - `all_star_model.ipynb`: A Jupyter Notebook containing the creation of the All-Star predictive model

## Coming soon
I am actively working on the following components to provide a more comprehensive analysis:
- `clustering.ipynb`: A Jupyter Notebook covering machine learning clustering analysis with scikit-learn.
- `all_star_model.ipynb`: A Jupyter Notebook containing the creation of the all-star predictive model
- `all_star_snubs.csv`: A list of the biggest all-star snubs in the last 5 years.

Stay tuned for more updates as I delve deeper into the exciting world of NBA data analysis


