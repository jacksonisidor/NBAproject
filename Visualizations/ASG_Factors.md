# Preliminary Analysis of Season Statistics and All-Star Selections

## Introduction
Part of this project includes building a model that can accurately predict all-star selections for a given season. To create an effective model, I must determine what factors are most important in a player becoming all-star.
As a preliminary check, I produced a few visualizations in Tableau to gain insight towards what makes an NBA all-star. Using this information, I will perform the proper statistical tests to find exact correlations to build an accurate model.

#### Note: 
These will include generally more advanced or unexpected statistics because we know the importance of the basic counting stats, like points, rebounds, and assists.  Also, my model will attempt to stick to relative statistics (ex. per game or per 100 possessions) as I do not have pre-all-star game statistics. Using full season totals would decrease it's reliability when I obtain first half of the season statistics for the upcoming year. 

## Visualizations

#### Vorp
- The scatterplot below illustrates the relationship between Value Over Replacement Player (VORP) and all-star status for all NBA players throughout league history. This is one of my favorite statistics and I expect it to be an important factor in predicting all-star games. This metric directly determines a players value added to their team compared to being replaced by another player. The x-axis 'Count' is just each players index to spread out the data points and make it more clear. The important information is the vertical placement and color of the points. I filtered for seasons from 1973 and on because that is the year the stastic began tracking.
- Players higher on the chart have a larger impact relative to the replacement-level. This directly indicates the most valuable players in the NBA, and this is important because you would expect all-stars players to be irreplacable and much better than replacement-level. 

<img src="https://user-images.githubusercontent.com/108153124/260272810-bbcff149-31d9-4805-8c6b-f69615314704.png" alt="Usage Percentage vs Minutes Per Game" width="400" height="500">

As expected,the top of the graph is exclusively all-stars, indicating that VORP should be a strong factor in determining all-stars. 


#### Usage Percentage and Minutes Per Game
- The scatterplot below demonstrates how Usage Percentage (Usg%) and Minutes Per Game (MPG) relate to all-star selections for NBA players of the past two seasons. Both of these statistics can be misleading with a small sample size, so I filtered for only the players that havef played at least 30 games.
- The visualization helps us understand how often a player is involved in their team's offensive plays (Usg%) and how much they are on the court (MPG) to establish their role to the team. Players in the top right corner of the scatterplot have high Usg% and MPG, indicating that they spend a significant amount of time on the court, and are very involved while out there.

<img src="https://user-images.githubusercontent.com/108153124/260263092-0c1d690f-4f59-430d-8368-31dfc0839d80.png" alt="Usage Percentage vs Minutes Per Game" width="400" height="500">

The concentration of All-Star players in the top right corner suggests that All-Stars are often heavily relied upon by their teams in terms of both usage and playing time.

#### Offensive Box Plus-Minus and Defensive Box Plus-Minus
- The scatterplot below depicts the relationship Offensive Box Plus Minus (OBPM) and Defensive Box Plus Minus (DBPM) have with all-star selections for NBA players of the past two seasons.
- Offensive/Defensive BPM measures a players impact based on the teams performance while they are on the court (in terms of points) per 100 possessions. This can help determine how valuable a players offensive impact, defensive impact, or both contribute to their all-star status. Players in the top right corner of the scatterplot have high OBPM and DBPM, indicating that their team performs very well on both ends of the court when they play compared to when they don't.
- As these are calculated per 100 possessions, both can be misleading with a small sample size, so I filtered for only the players that have played at least 30 games.
  
<img src="https://user-images.githubusercontent.com/108153124/260263141-2b703c40-8012-4b11-9548-208e20d116ba.png" alt="Offensive Box Plus-Minus vs Defensive Box Plus-Minus" width="400" height="500">

Nearly all of the all-stars are on the right side, indicating a positive OBPM is essential to being selected as an all-star. DBPM, on the other hand, seems to be more spread out in terms of positive and negative. It appears most all-stars have a positive DBPM, but I will need to run more tests to know its actual significance. 

#### Offensive Win Shares Per 48 and Defensive Win Shares Per 48
- The scatterplot below displays how Offensive Win Shares Per 48 Minutes (OWS/48) and Defensive Win Shares Per 48 Minutes (DWS/48) relate to all-star selections for NBA players since 1980. Win shares attribute a portion of a player's team success, accruing over the course of the season. WS/48 calculates a player's win shares per 48 minutes of play.
- OWS/48 and DWS/48 measures a players average contribution to the teams success, therefore quantifying the players impact directly with success. Players in the top right corner of the scatterplot have high OWS/48 and DWS/48, indicating that they are responsible for much of their teams offensive and defensive success.
- This statistic can be easily skewed with a small sample size (imagine a players win shares getting larger because they haven't even played 48 minutes). To remedy this, I filtered for only players who played at least 30 games.

<img src="https://user-images.githubusercontent.com/108153124/260326903-4c070cac-a651-4bda-a763-82ad1677dc27.png" width="400" height="500">

The concentration of all-stars in the right quadrant is evident. However, their distribution is fairly diverse — some all-stars have high OWS/48 and low DWS/48, while others exhibit the reverse. Additionally, many players showcase a combination of both. This observation suggests that the total WS/48 (OWS/48 + DWS/48) might serve as a more comprehensive statistic for consideration, as it appears to be the common factor among the all-stars.

#### Win Percentage and Number of Starts
- This scatterplot illustrates how team win percentage and total number of starts relate to all-star selections for NBA players of the past two seasons. Win% represents the players win percentage for the full season, but all-stars are selected before the halfway point. I do not have statistics for strictly pre-ASG, so full season win% should suffice because most teams do not drastically change their win% between the first and second half of the season for it to have too much of an effect. Another potential issue I encountered came with players that switched teams during the season. I have no data on which games they played for which teams and the results of those specific games. To remedy this, I gave them the league average win% because I predict win% to not a major determining factor in all-star selection. I expect win% to be more of a minimum threshold for all-star selection, i.e. not be on the worst team in the league. 
- Win% measures a players team success and starts roughly indicates how important they were to the team. These two together measures a concept similar to win shares, but with a bit less complexity. Players in the top right corner of the scatterplot have a high win% and a lot of starts, implying that they are a valuable player on a top team. This distinction is roughly what you would expect an all-star to be. 

<img src="https://user-images.githubusercontent.com/108153124/260263140-17000782-a2fe-4025-b3ed-9acc592b4099.png" alt="Win Percentage vs. Number of Starts" width="400" height="500">

As I predicted, both win% and starts appear to have a minimum threshold requirement for being an all-star. All all-stars have at least 40 starts and a 40% win percentage. Keep in mind, those are for the 82 game season. The players closer to only 40 starts may have played the whole first half of the season, selected as an all-star, then injured for the second half of the season. 

#### All-Star's Experience Level
- This bar chart shows the experience each NBA player when they made the all-star game throughout the history of the league.
- Age may be a valuable factor in determining whether a player is an all-star or not. Looking at peaks in the chart can show periods where players make the all-star game most frequently. 

<img src="https://user-images.githubusercontent.com/108153124/260263143-2f9109d5-4b10-4872-b974-96fc57145c25.png" alt="All-Star's Experience Level" width="400" height="500">

Players with 5 years of experience have made the all-star game the most, with the majority being between 3 and 7 years. Despite the clear bell-shaped chart indicating a potential factor, I am hesitant to include it in my model. This is because I do not know if experience itself is truly the determining factor in being an all-star. I would argue it is more likely that this level of experience/age is when players perform the best, and therefore get selected based on that peformance. For example, I expect a player with less experience to make the all-star game if they perform as well as someone older. Basically, I believe including all the other performance metrics negates the need for experience level as a factor.

## Conclusion
These preliminary visualizations provide valuable insights into the factors that contribute to all-star selections. VORP, usage percentage, minutes per game, offensive and defensive metrics, win percentage, and starts all appear to influence all-star status. This initial analysis will guide further statistical tests evaluating factors to build a robust all-star prediction model.
