<p align="center">
  <img src="https://github.com/rob-field/Euro2021-ML-Predictions/blob/main/euros2021.png" />
</p>

# Euro2021-Predictions
Aim: Using past international fixtures predict the results and outcome of the UEFA Euros 2020/21 competition.

# Data and Method
A Logistic Regression model is fitted and tuned (using RandomisedSearchCV) using past international results from all competitions from a kaggle dataset (https://www.kaggle.com/martj42/international-football-results-from-1872-to-2017). Predictive outcomes (win/lost/draw) and  predictive probabilities are then generated using the model for the Euro2021 fixtures (https://fixturedownload.com/results/uefa-euro-2020).  
Fifa club/team rankings were also appended to the dataset (https://www.fifa.com/fifa-world-ranking/ranking-table/men/) as an additional feature to improve predictive power.  

The model predicted that Belgium would be the overall winner.  

# Improvements  
Different models, such as XGBoost or LightGBM could also be used to improve predictive power, however these are more scoring metrics would have to be evaluated and they are more computationally taxing.  
Additional data features could be collected to improve the models predictive power, such as referees, stadium and even macth odds from various betting sites.

# Packages/Environment
Python 3.7.10  
Jupyter Lab  
SK-Learn  
numpy  
pandas  
