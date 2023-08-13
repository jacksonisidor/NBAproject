# Preliminary Analysis of Season Statistics and All-Star Selections

## Introduction
Part of this project is building a model that can accurately predict all-star selections for a given season. To create an effective model, I must determine what factors are most important in a player becoming all-star.
As a preliminary check, I produced a few visualizations in Tableau to gain insight towards what makes an NBA All-Star. Using this information, I will perform the proper statistical tests to find exact correlations to build an accurate model.

## Visualizations

### Vorp (Scatterplot)
<img src="https://imgur.com/1BObxWE" alt="VORP Relationship with ASG" width="400" height="500">

  - **Description:** This scatterplot illustrates the relationship between Value Over Replacement Player (VORP) and all-star status for all NBA players throughout league history. This is one of my favorite statistics and I expect it to be an important factor in predicting all-star games. This metric directly determines a players value added to their team compared to being replaced by another player. The x-axis 'Count', which is basically just each players index. I did this to spread out the data points and make it more clear. The important information is the vertical placement and the color of the points. I filtered for seasons from 1973 and on because that is the year the stastic began tracking. 
  - **Significance:** The visualization helps us understand not only how good a team is with the player, but the difference between their value and a replacement players value, which shows clearly how much they bring to the team. 
  - **Insights:** Players higher on the chart have a larger impact relative to the replacement-level. This directly indicates the most valuable players in the NBA, and this is important because you would expect all-stars players to be irreplacable and much better than replacement-level. 
  - **Analysis:** As expected,the top of the graph is exclusively all-stars, indicating that VORP should be a strong factor in determining all-stars. 


### Usage Percentage vs Minutes Per Game (Scatterplot)
<img src="https://user-images.githubusercontent.com/108153124/260263092-0c1d690f-4f59-430d-8368-31dfc0839d80.png" alt="Usage Percentage vs Minutes Per Game" width="400" height="500">

  - **Description:** This scatterplot illustrates how Usage Percentage (Usg%) and Minutes Per Game (MPG) relate to all-star selections for NBA players of the past two seasons. Both of these statistics can be misleading with a small sample size, so I filtered for only the players that havef played at least 30 games. 
  - **Significance:** The visualization helps us understand how often a player is involved in their team's offensive plays (Usg%) and how much they are on the court (MPG) to establish their role to the team. 
  - **Insights:** Players in the top right corner of the scatterplot have high Usg% and MPG, indicating that they spend a significant amount of time on the court, and are very involved while out there. 
  - **Analysis:** The concentration of All-Star players in the top right corner suggests that All-Stars are often heavily relied upon by their teams in terms of both usage and playing time.

### Offensive Box Plus-Minus vs Defensive Box Plus-Minus (Scatterplot)

<img src="https://user-images.githubusercontent.com/108153124/260263141-2b703c40-8012-4b11-9548-208e20d116ba.png" alt="Offensive Box Plus-Minus vs Defensive Box Plus-Minus" width="400" height="500">

  - **Description:** This scatterplot illustrates how Offensive Box Plus Minus (OBPM) and Defensive Box Plus Minus (DBPM) relate to all-star selections for NBA players of the past two seasons. Both of these statistics can be misleading with a small sample size, so I filtered for only the players that havef played at least 30 games. 
  - **Significance:** Offensive/Defensive BPM measures a players impact based on the teams performance while they are on the court (in terms of points). This can help determine how valuable a players offensive impact, defensive impact, or both contribute to their all-star status. 
  - **Insights:** Players in the top right corner of the scatterplot have high OBPM and DBPM, indicating that their team performs very well with them on the court. 
  - **Analysis:** Nearly all of the all-stars are on the right side, indicating a positive OBPM is essential to being selected as an all-star. DBPM, on the other hand, seems to be more spread out in terms of positive and negative. It appears most all-stars have a positive DBPM, but I will need to run more tests to know its actual significance. 

### Offensive Win Shares vs Defensive Win Shares (Scatterplot)

<img src="https://user-images.githubusercontent.com/108153124/260263138-025338d9-0892-4ed4-b6cc-20e6696c82df.png" alt="Offensive Win Shares vs Defensive Win Shares" width="400" height="500">

  - **Description:** This scatterplot illustrates how Offensive Win Shares (OWS) and Defensive Win Shares (DWS) relate to all-star selections for NBA players of the past two seasons. Win shares credits players with a share of their teams success, accumulating throughout the season. As this statistics is additive, I do not need to filter based on games played.
  - **Significance:** OWS and DWS measures a players contribution to the teams success, therefore quantifying the players impact directly with success. 
  - **Insights:** Players in the top right corner of the scatterplot have high OWS and DWS, indicating that they are responsible for much of their teams offensive and defensive success.
  - **Analysis:** All of the all stars appear to have a high total win shares (add up their OWS and DWS), whether its a high OWS and low DWS, vice versa, or a combination of both. This means that total win shares may be a better statistic to predict all-star status.

### Win Percentage vs. Number of Starts (Scatterplot)

<img src="https://user-images.githubusercontent.com/108153124/260263140-17000782-a2fe-4025-b3ed-9acc592b4099.png" alt="Win Percentage vs. Number of Starts" width="400" height="500">

  - **Description:** This scatterplot illustrates how team win percentage and total number of starts relate to all-star selections for NBA players of the past two seasons. Win% represents the players win percentage for the full season, but all-stars are selected before the halfway point. I do not have statistics for strictly pre-ASG, so full season win% should suffice because most teams do not drastically change their win% between the first and second half of the season for it to have too much of an effect. Another potential issue I encountered came with players that switched teams during the season. I have no data on which games they played for which teams and the results of those specific games. To remedy this, I gave them the league average win% because I predict win% to not a major determining factor in all-star selection. I expect win% to be more of a minimum threshold for all-star selection, i.e. not be on the worst team in the league. 
  - **Significance:** Win% measures a players team success and starts roughly measures how important they were to the team. These two together measures a concept similar to win shares, but with a bit less complexity.  
  - **Insights:** Players in the top right corner of the scatterplot have a high win% and a lot of starts, indicating that they are a valuable player on a top team. This distinction is roughly what you would expect an all-star to be. 
  - **Analysis:** As I predicted, both win% and starts appear to have a minimum threshold requirement for being an all-star. All all-stars have at least 40 starts and a 40% win percentage. Keep in mind, those are for the 82 game season. The players closer to 40 starts may have played the whole first half of the season, selected as an all-star, then injured for the second half of the season. 

### All-Star's Experience Level (Bar Chart)

<img src="https://user-images.githubusercontent.com/108153124/260263143-2f9109d5-4b10-4872-b974-96fc57145c25.png" alt="All-Star's Experience Level" width="400" height="500">

  - **Description:** This bar chart illustrates the experience each NBA player when they made the all-star game throughout the history of the league.
  - **Significance:** Age may be a valuable factor in determining whether a player is an all-star or not. 
  - **Insights:** Looking at peaks in the chart can show periods where players make the all-star game most frequently. 
  - **Analysis:** Players with 5 years of experience have made the all-star game the most, with the majority being between 3 and 7 years. Despite the clear bell-shaped chart indicating a potential factor, I am hesitant to include it in my model. This is because I do not know if experience itself is truly the determining factor in being an all-star. I would argue it is more likely that this level of experience/age is when players perform the best, and therefore get selected based on that peformance. For example, I expect a player with less experience to make the all-star game if they perform as well as someone older. Basically, I believe including all the other performance metrics negates the need for experience level as a factor.
