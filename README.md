# About

## Sequence-to-Sequence Frequency model used to predict Python code. Dataset given consisted of tokenized python code with 
method headers and invocators identified to eliminate the process of parsing on the participants' end. The goal is to give
the top 5 suggestions whenever a "TOKEN_TO_PREDICT" is encountered in the tokenized files. 

## Approach was initially to use a Compact Prediction Tree but later optimized to eliminate the use of a tree in favor of a 
list. This is because any sequence is guaranteed to be 2 elements long with the first being the method header and the second
being the method invocator. It was unncessary to traverse through a tree with every retrieval of a method invocator. Using a
list allows for constant retrievals, and thus, faster when there are over hundreds of thousands of sequences (even millions).

Sources:
https://www.analyticsvidhya.com/blog/2018/04/guide-sequence-prediction-using-compact-prediction-tree-python/
