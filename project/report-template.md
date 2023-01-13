# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Barbara Stefanovska

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
100% of the work was done in SageMaker so things went very smooth. I had sam problems with instalation but later realized I forgot to se the autogluon version to 0.2.0 . As soon as I fixed this the process could start. I set the parametars as given in the task and got the "initial" score of  1.36777.

### What was the top ranked model that performed?
The top ranked model was the model after I did the hyperparametar tuning with a score of 0.47601.

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
As suggested in the task I split the datetime feature into hour day and month which significazntly improved my model. I also counted the negative values and replaced them with zeros. 

### How much better did your model preform after adding additional features and why do you think that is?
It improved from 1.3677 to 0.51086. This is a significant improvement in the result, and mostley due to the high impact that the month-in-the-year and hour-in-the-day has on the amounts of bikes rented versus looking at the merged feature of datetime.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
It improved by appeoximatley 0.1, which is good. Unfortunatley I did not menage to understand the hyperparameter tuning part, nor did I have enough information to be able the full potential to my advantage more.

### If you were given more time with this dataset, where do you think you would spend more time?
I would definetley give more time to Exploratory data analysis as well as learn hyperparameter tuning more in dept, as I think theese two parts cans ignificantly improve the model.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|?|?|?|?|
|add_features|?|?|?|?|
|hpo|?|?|?|?|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.


![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary
TODO: Add your explanation
