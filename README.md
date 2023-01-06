# santander_customer_satisfaction
 
This repo contains data from kaggle that is titled santander customer satisfaction which is from a competion 6 years ago where santander has provided a lot of data without any variable names to the dataset.
It has 370 different variables in total, so the initial goal was to reduce this variables to less than 100 and then build a few models to get the best score.
One major problem with this dataset is that it is highly imbalanced, so metrics like accuracy do not work in this case hence the choice of roc_auc for this project.
Initially all the constant and quasi-constant coulmns are dropped and then corellated colums are also dropped only keeping one in each pair.
Then, decison tree classifier is built using differnet configurations but no imporovement observed with the score which is pretty low.
To counter the imbalance further SMOTE has been then introduced to the dataset and a significant improvment in the roc score is observed.
Then, coming to the final models XGBoost is chosen and GridCV is run multiple times and the model is finetuned to get a satisfactory score that is close to the kaggle leaderboard.

