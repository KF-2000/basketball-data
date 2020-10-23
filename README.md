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
