# IPL_Score_Predictor
Innings score predictor using simple linear regression and ridge regression model.

The dataset contains the match record ball by ball for every match between IPL 2008 - IPL 2017

<img width="1033" alt="image" src="https://user-images.githubusercontent.com/44739430/185656327-5d249913-ddc3-4648-9916-7ab3ef4c72ef.png">

We try to pre-process few columns and clean some data and finally use the following parameters
1. Match Date
2. Batting Team
3. Bowling Team
4. Runs per ball
5. Wickets per ball
6. Runs in Last 5 overs
7. Wickets in Last 5 overs
8. Total Score in that innings
<img width="707" alt="image" src="https://user-images.githubusercontent.com/44739430/185656601-08b857f4-a571-4bd0-8782-547cb1faa0b7.png">

We do some more pre-processing and cleaning the data and maintaining some consistency among matches played between various teams.

Then we perform Linear Regression as well as Ridge Regression on the same dataset and compute the prediction. So that a comparative study can be done about which method gives a better prediction in these kind of volatile scenario.

The error given by Ridge Regression was lower than that of linear Regression.

The probability density function curve obtained is shown below.

<img width="305" alt="image" src="https://user-images.githubusercontent.com/44739430/185662293-2236f577-b8d7-4206-aaac-4dee112a5204.png">

Finally in order to get a score-prediction output based on any situation in a match the following parameters were taken as input from the user
1. Batting Team
2. Bowling Team
3. Overs Played (Should be greater than 5 in order to get a prediction)
4. Runs Scored till that over
5. Wickets Fallen
6. Runs in the last 5 overs
7. Wickets in the last 5 overs

<img width="309" alt="image" src="https://user-images.githubusercontent.com/44739430/185662909-c50af49d-9e81-4292-b068-04ee550edf3b.png">

Based on the above conditions a score predicion is given by the model. This model gives an accuracy of 88%.
