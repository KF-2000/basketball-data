# basketball-data
Scraping basketball statistics and employing a linear regression model in order to predict how many points a player will score in a game.

### Description

The purpose of this repository is to create a place for me to document my experimentation with collecting basketball data from basketball-reference.com.
The number of points a player scores in a game, is one of the most important factors to winning a game of basketball as the aim is to, well, score more than your opponent. For
gambling or fantasy sports predicting how well your scorers will score is an important factor when making decisions on what bets you want to place or which players you want to 
put your faith in.

In this project, I've initially done some feature engineering in order to refine the number of statistical categories that I will use in my regression model. The initial statistics
that I think have the most affect on a player's point production are: field goals made FG, field goals attempted FGA, three pointers made 3P, three pointers attempted 3PA, 
free throws made FT, free throws attempted FTA, usage percentage USG% and offensive rating ORtg.

I'll be creating an ordinary least squares model to create my first model for points production. Next I'll employ a weighted least squares model applying the weights as required for
each type of goal (two point field goals, three point fields goals, and free throws worth on point). Finally, I'll look at using a neural network and experiment which activation functions,
and optimisation functions work best for the model.

### Condclusions

After completing the notebooks for this repository, I've found that although I wasn't able to make any interesting insights regarding the relationships between my chosen metrics (point scoring features that directly contributing to the total points scored by a player.) however I think this was a good first exercise to not only employ what I've learnt in pandas and scikit-learn to large datasets, but also to explore the ways in which keras can be used to develop a neural network and experiment with the architecture of my neural networks for the problem I'm considering.
In the future it may be more interesting to increase the complexity of this model, by not only considering statistics that are positively contributing to scoring (e.g. an attacking team/player's field goals scored, shooting percentages, advanced offensive metrics), but also statistics negatively contributing to scoring (e.g. the defending team's blocks per possession, steals per possession, defensive rebounds). This would be a much more complex problem as I would have to consider the average times each team/player gain possession of the ball and then exploring the probability or total contributions to whether the score changes favourably or unfavourbly for each side. 
