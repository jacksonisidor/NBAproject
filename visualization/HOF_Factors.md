# Preliminary Analysis of Career Statistics and Hall of Fame Inductions

## Introduction
This project involves constructing predictive models to assess both retired players' Hall of Fame eligibility and active players' likelihood of entering the Hall of Fame. To establish an effective model, identifying the key factors influencing a player's induction into the Hall of Fame is crucial. As a preliminary step, I generated visualizations using Tableau to glean insights into the attributes that distinguish NBA Hall of Famers. These insights will guide me into the next step of conducting precise statistical analyses aimed at uncovering correlations necessary for building an accurate predictive model.

#### Notes: 
- All of these visualizations have been filtered for players eligible for the Hall of Fame, meaning players that played their last season in 2019 or earlier. 
- These will include mostly accolades and some other statistics outside of points, rebounds, and assits because we know the importance of the basic counting stats. In regard to those, my model will test both per game and total statistcs to see what works best.

## Visualizations

#### Total All-Star Selections
- The stacked bar chart below illustrates the relationship betwen number of all-star appearances and Hall of Fame status. The count represents the number of all stars an individual player has and the length of the yellow bar represents the percentage of players in the Hall of Fame within that count.
<img src="https://user-images.githubusercontent.com/108153124/260297862-dac55850-b804-4ef0-8376-092bb9be375f.png" width="400" height="400">
This clearly shows that a higher percentage of players with multiple all-stars making the Hall of Fame. The rate of Hall of Famers is low (below 10%) for players with 1 to 3 all-star appearances, but jumps dramatically to 40% at 4 all-star selections. This rate continues to rise quickly - every player with at leaset 7 all-star games, except for one (Larry Foust), is in the Hall of Fame.

#### Total MVP Awards
- The stacked bar chart below displays the percentage of players that are in the Hall of Fame within each count of Most Valuable Player (MVP) awards.
<img src="https://user-images.githubusercontent.com/108153124/260278946-fa602a2d-c75e-4c0e-a5d2-efd7a93fd721.png" width="400" height="400">
This shows us something very important - every single player that has one at least 1 MVP, and is eligible, is in the Hall of Fame. This will become very useful in predicting what players are in the Hall of Fame, and what current players have the best chance of making it after retirement.

#### Total DPOY Awards
- The stacked bar chart below represents the percentage of players in the Hall of Fame for each Defensive Player of the Year (DPOY) award recieved.
<img src="https://user-images.githubusercontent.com/108153124/260278948-e685f23e-00fe-4d2a-8308-3d84c580dc9f.png" width="400" height="400">
This shows a steady increase in Hall of Fame percentage for each additional DPOY. However, there is limited data to work with as only 2 players have won 4 DPOY and 0 players have won 3 (that are eligible for HOF).

#### Games and Win Percentage
- This scatterplot shows how career games played and win percentage relate to Hall of Fame status.
- These two statistics can show how relevant longevity and team success is to being inducted into the Hall of Fame.
<img src="https://user-images.githubusercontent.com/108153124/260278953-8508d31d-3bd6-49f0-bd5e-8c13f221155b.png" width="400" height="400">
I expected longevity and team success to be a huge factor because people debate it all the time. However, it appears these two factors are not much different for HOFers and non-HOFers. The Hall of Fame points may be a bit further to the right and top, but it is not clear. I believe it still worth testing.

#### Offensive Win Shares and Defensive Win Shares
- This scatterplot depicts the correlation between offensive win shares (OWS) and defensive win shares (DWS), and their relationship with Hall of Fame status. Win shares credits players with a share of their teams success, accumulating throughout their career.
- OWS and DWS measures a players contribution to the teams success, therefore quantifying the players impact directly with success. Players in the top right corner of the scatterplot have high OWS and DWS, indicating that they are responsible for much of their teams offensive and defensive success.
<img src="https://user-images.githubusercontent.com/108153124/260278949-4b66adb6-c4b4-435b-9d94-3b8329b2f61f.png" width="400" height="400">
All of the Hall of Fame appear to have a high total win shares (add up their OWS and DWS), whether its a high OWS and low DWS, vice versa, or a combination of both. This means that total win shares may be a better statistic to predict Hall of Fame status. This is not too surprising, as I found the same results in the ows vs. dws visualization for all-stars.

## Conclusion
This preliminary analysis lays the groundwork for predicting NBA Hall of Fame inductions. By exploring career statistics and visualizing key attributes using Tableau, I have gained initial insights into the factors that contribute to Hall of Fame status. As I move forward, these insights will guide my in-depth statistical analysis to establish accurate correlations between attributes and Hall of Fame induction. This process will enable us to develop effective predictive models for both retired and active players, contributing to a deeper understanding of the criteria behind NBA Hall of Fame honors.
