# test_test

Presentation Slides: https://docs.google.com/presentation/d/e/2PACX-1vTAMfLWzf2zl8dotI97XZkTi_rhz3TOu-r6kGnKJQIdqD6a8xkzPZJgN7XnLE-WXA6YLvhv6_G2GDBa/pub?start=false&loop=false&delayms=30000

ALL-NBA TEAM PREDICTOR

EXPLANATION FOR ALL-NBA TEAM

-An annual honor given to best players in the league

-Comprised of 3 teams - 1st Team, 2nd Team, 3rd Team

-Each team consists of  2 guards, 2 forwards, 1 center

-Teams are voted on by panel of sportswriters and broadcasters.

OBJECTIVE

Build machine learning model to predict All-NBA Team and check if it’s possible even with partial 2023 data 

DATA CLEANSING

First we acquired three CSV files containing our data from Kaggle (source: Basketball-Reference.com).
The data was merged into a single CSV file and then organized into a dataframe. The data was then searched for any null or duplicate values, which were dropped.
In the dataset, there were multiple categories for the positions of the players. The extra categories were for players who played multiple positions and were displayed as combinations of forward, guard, and center.
This issue was resolved by narrowing the categories down to just forward, guard, and center and by notating the player's participation in each of the positions with a boolean value.

DATA POINTS

  Player Data

    -Position
  
    -Age
  
    -Experience
  
    -Games played/started
  
    -Minutes played
  
    -FG attempted/made
  
    -3FG attempted/made
  
    -FT attempted/made
  
    -Points
  
    -Rebounds
  
    -Assists
  
    -Steals
  
    -Blocks

  End of Year Awards

    -Season
  
    -All NBA Selections

  Team Summary

    -Season
    
    -Win/Loss record

STEPS TO SUCCESS

After preparing our data, any categorical variables were converted into indicator variables, then scaled.
The data was split into testing and training sets and a standard scaler was used to scale these features. The scaler was then trained with our training data.
A logistic regression was used for this model and after training it, our model produced a training data score of 98.85% and a testing data score of 98.60%.


2023 PREDICTION

Once our model had been refined and reached a meaningful predictive power 
of 98% classification accuracy, it was used to predict the All-NBA Team for 2023. The results of this prediction include 15 players total with 6 guards, 6 forwards, and 3 centers.

GUARD PREDICTIONS
1. Luka Dončić - Dallas Mavericks
2. Ja Morant - Memphis Grizzlies
3. Shai Gilgeous-Alexander - Oklahoma City Thunder
4. Damian Lillard - Portland Trail Blazers
5. Trae Young - Atlanta Hawks
6. James Harden - Philadelphia 76ers

FORWARD PREDICTIONS
1. Giannis Antetokounmpo - Milwaukee Bucks
2. Jayson Tatum - Boston Celtics
3. Julius Randle - New York Knicks
4. Jaylen Brown - Boston Celtics
5. LeBron James - Los Angeles Lakers
6. Kevin Durant - Phoenix Suns

CENTER PREDICTIONS
1. Nikola Jokić - Denver Nuggets
2. Joel Embiid - Philadelphia 76ers
3. Domantas Sabonis - Sacramento Kings

POTENTIAL LIMITATIONS

Human Error/Bias: The All-NBA team is voted on by NBA media members. There is no set criteria for the 15 players selected so voter bias could potentially destroy our prediction.
Partial Season Data: Our data originated with about 25 games remaining in the season. Our model wasn’t able to take into account injuries that happened after our data was pulled.

LINKS

Tableau Presentation: https://public.tableau.com/app/profile/edward.spiezio.runyon/viz/UTSA-Project-4-All-NBA-Team-Predictor/All-NBAPredictions

Data: https://basketball-reference.com

NBA Logos: https://www.sportslogos.net/teams/list_by_league/6/National_Basketball_Association/NBA/logos/


<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vTAMfLWzf2zl8dotI97XZkTi_rhz3TOu-r6kGnKJQIdqD6a8xkzPZJgN7XnLE-WXA6YLvhv6_G2GDBa/embed?start=true&loop=false&delayms=5000" frameborder="0" width="1440" height="839" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
