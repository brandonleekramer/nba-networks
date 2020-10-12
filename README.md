### NBA Networks

This objective of this project is to use machine learning to examine trends about NBA players and teams. Although I plan to develop statistical models for future performance of both NCAA prospects and current NBA players, I am also hoping to levearage a graph-based machine learning approach to examine player-team transitions like free agency movement and trades. 

### Checklist

Original model takes boxscore college stats (G, GS, MP, FG, FGA, FG%, 2P, 2PA, 2P%, 3P, 3PA, 3P%, FT, FTA, FT%, ORB, DRB, TRB, AST, STL, BLK, TOV, PF, PTS, SOS, Year, Pos, Age) and attempts to predict NBA career outcome to date (NBATRB, NBAAST, NBASTL, NBABLK, NBAPTS). My ultimate goal is to use this for fantasy purposes, which requires changing the outcomes to fantasy points based on different leagues or ranks based on which cats I care about. Moreover, I would want to add information about team situation (past winning percentage, projected winning percentage, average age of team, etc.) as well as player data, including biometrics information, draft position, a proxy for injury information during college or in their early NBA career (e.g. Jay Williams). I'd also want to update the career aspect of these projections. I'm more interested in peak performance as well as peak money value. For example, if a player is performing strongly but is still on a rookie contract, they might have more value in fantasy than someone that outscores them at a higher contract. From past research, I know that future stars on the last two years of their rookie year are the most valuable asset in points leagues, so I would want to hone my model to predict best performance for NBA players in their 2nd-4th years instead of entire career. 

- Add fantasy composites for local cats and points leagues 
- Add contract values for local leagues (raw money)
- Develop a new value function that accounts for top-tier players contributing more points at higher contracts 
- Add all individual player data from each year (and then filter to only include 2nd-4th years)
- Normalize outcomes based on actual NBA team winning percentage, age, and project winning percentage 
- Could add in consensus scouting reports (from KOC and other mock drafts listed online)

### Performance Data  

[NBA Basketball Reference Stats](https://www.kaggle.com/drgilermo/nba-players-stats)
[Open-Source Sports Professional Baseketball Stats](https://www.kaggle.com/open-source-sports/mens-professional-basketball)
[Aggregated Kaggle datasets](https://www.kaggle.com/data/52669)
[Advanced box score and standings (2012-2018)](https://www.kaggle.com/pablote/nba-enhanced-stats#)

### Network Data 

[Pro Sports Transactions Data for Trades Over Time](http://www.prosportstransactions.com/)
[Potential code for scaping Protransactions data](https://github.com/svitkin/bball-trade-network)

### Existing Examples 

**Daniel, J. (2020). "Predict NBA Draft using Machine Learning!" *Medium.* [Paper.](https://medium.com/analytics-vidhya/predict-nba-draft-using-machine-learning-7023503e33e7) [GitHub.](https://github.com/Jwdaniel34/Drafting_college_players)** 

Drawing on data from 30,000+ college and 4,450 NBA players, Daniel (2020) uses 27 features to develop a binary classifier to predict likelihood of NCAA players getting drafted. He finds games played, 2P% and FT% to be the most robust predictors with assists, blocks, steals, minutes and games started in the next tier.

**Kannan, S. (2019). "Predicting NBA Rookie Stats with Machine Learning." [Medium.](https://towardsdatascience.com/predicting-nba-rookie-stats-with-machine-learning-28621e49b8a4) [GitHub.](https://github.com/SidTheKid007/NBARookieAnalysis)**

**Kannan et al. (2018). "Predicting National Basketball Association Success: A Machine Learning Approach." *SMU Data Science Review.* [Paper.](https://scholar.smu.edu/cgi/viewcontent.cgi?article=1033&context=datasciencereview)**

**Tabtah et al. (2019). "NBA Game Result Prediction Using Feature Analysis and Machine Learning" *Annals of Data Science.* [Paper.](https://link.springer.com/article/10.1007/s40745-018-00189-x)**

**Aybul, K. (2020). "Draft Ranking Based on Scouting Consensus" [Reddit](https://www.reddit.com/r/NBA_Draft/comments/j4m08k/i_built_a_statistical_model_that_projects/?utm_source=share&utm_medium=ios_app&utm_name=iossmf) [Google Sheet](https://docs.google.com/spreadsheets/d/1YmPsiD5t_IWeqQc9Zig7LJ4nBjVUL7BIixmym-6Ei0Y/edit#gid=1511007488) **