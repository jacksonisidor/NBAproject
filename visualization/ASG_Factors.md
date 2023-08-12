# Preliminary Analysis of Season Statistics and All-Star Selections

## Introduction
Part of this project is building a model that can accurately predict all-star selections for a given season. To create an effective model, I must determine what factors are most important in a player becoming all-star.
As a preliminary check, I produced a few visualizations in Tableau to gain insight towards what makes an NBA All-Star. Using this information, I will perform the proper statistical tests to find exact correlations to build an accurate model.

## Visualizations

### Usage Percentage vs Minutes Per Game (Scatterplot)
<img src="https://user-images.githubusercontent.com/108153124/260263092-0c1d690f-4f59-430d-8368-31dfc0839d80.png" alt="Usage Percentage vs Minutes Per Game" width="400" height="500">

  - **Description:** This scatterplot illustrates how Usage Percentage (Usg%) and Minutes Per Game (MPG) relate to all-star selections for NBA players of the past two seasons. Both of these statistics can be misleading with a small sample size, so I filtered for only the players that havef played at least 30 games. 
  - **Significance:** The visualization helps us understand how often a player is involved in their team's offensive plays (Usg%) and how much they are on the court (MPG) to establish their role to the team. 
  - **Insights:** Players in the top right corner of the scatterplot have high Usg% and MPG, indicating that they spend a significant amount of time on the court, and are very involved while out there. 
  - **Analysis:** The concentration of All-Star players in the top right corner suggests that All-Stars are often heavily relied upon by their teams in terms of both usage and playing time.

### Offensive Box Plus-Minus vs Defensive Box Plus-Minus (Scatterplot)

<img src="https://user-images.githubusercontent.com/108153124/260263141-2b703c40-8012-4b11-9548-208e20d116ba.png" alt="Usage Percentage vs Minutes Per Game" width="400" height="500">

  - **Description:** This scatterplot illustrates how Offensive Box Plus Minus (OBPM) and Defensive Box Plus Minus (DBPM) relate to all-star selections for NBA players of the past two seasons. Both of these statistics can be misleading with a small sample size, so I filtered for only the players that havef played at least 30 games. 
  - **Significance:** Offensive/Defensive BPM measures a players impact based on the teams performance while they are on the court (in terms of points). This can help determine how valuable a players offensive impact, defensive impact, or both contribute to their all-star status. 
  - **Insights:** Players in the top right corner of the scatterplot have high OBPM and DBPM, indicating that their team performs very well with them on the court. 
  - **Analysis:** Nearly all of the all-stars are on the right side, indicating a positive OBPM is essential to being selected as an all-star. DBPM, on the other hand, seems to be more spread out in terms of positive and negative. It appears most all-stars have a positive DBPM, but I will need to run more tests to know its actual significance. 
