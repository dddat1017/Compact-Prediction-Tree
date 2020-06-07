# About

Sequence-to-Sequence Frequency model used to predict Python code. The model utilizes a Compact Prediction Tree
to allow for ease of storing and retrieving predictions.

Dataset given consisted of tokenized Python code with method headers and invocators identified to eliminate the process of parsing on the participants' end. The goal was to give the top 5 suggestions whenever a "TOKEN_TO_PREDICT" is encountered in the tokenized files.

This project was completed during the Microsoft OneWeek Hackathon. Dataset was provided by the contest organizers.

## More on given Dataset ##
The tokenized Python code was extracted from roughly 2,000 starred Github repos.

References:
https://www.analyticsvidhya.com/blog/2018/04/guide-sequence-prediction-using-compact-prediction-tree-python/
