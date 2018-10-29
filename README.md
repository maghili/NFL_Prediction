# NFL_Prediction
Here we work with the historic data that is provided by FiveThirtyEight, on the historical predictions by ELO since 1920 <a href = "https://github.com/fivethirtyeight/data/tree/master/nfl-elo">here</a>. The predictions are not 100 percent accurate, but as a project what I want to do is to use the historical data to teach the machine and find the outcome of the future games given that I know what is ELO predictions.
In fact if we do some data analysis we find that the accuracy of ELO prediction is `65.352658212`, and it has a decreasing trend.
<img src = "https://github.com/maghili/NFL_Prediction/blob/master/pred.png">

For the games that the prediction probability was higher than 80 percent the accuracy seems to be much better

<img src = "https://github.com/maghili/NFL_Prediction/blob/master/highpred.png">

<h2>How to classify?</h2>
We add a correctly predicted class, and look at ELO predictions and winning probabilities. Whenever the winning probability by ELO gives the higher probability to the winner, we classify it as correct and set it to one and we set it to zero otherwise. Doing so we can use the Logistic Regression to find whether the prediction by ELO is correct or not. My model was able to do the prediction with 100 percent.
