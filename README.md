# udacityproj
Contain my learning projects on Udacity
# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Olanrewaju Abdulbasit

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: The evaluation score was negative which is -53.01
	I used the datetime and count for submission

### What was the top ranked model that performed?
WeightedEnsemble_L3

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
I see I could get more insight if I'm to split my datetime column  into hours and more and I did this with .dt.hour and as well rendered some column as category

### How much better did your model preform after adding additional features and why do you think that is?
The model perform better with -30.38 score and which is 42.6% increase, I think it is because of the added features

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
The model performed better with hyperparameter but not upto the one with added features score = # -36.33 #%increase = 31.46%

### If you were given more time with this dataset, where do you think you would spend more time?
I would add new features suh as datetime day, minutes and seconds
### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|default vals|default vals|default vals|1.80|
|add_features|default vals|default vals|default vals|0.63|
|hpo|NN epochs:[10]|GBM no. of leaves [26,66]|default vals|0.48|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

![model_train_score.png](/model_train_scorenn.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](/model_test_score.png)

## Summary
TODO: Apparently my kaggle submission score reduced but the model perform better with added features and hyperparameter tuning
