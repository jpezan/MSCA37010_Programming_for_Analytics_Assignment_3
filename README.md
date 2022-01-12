# MSCA37010n Programming for Analytics Assignment 3
## Hyper Parameter Optimization

##### Course: Programming for Analytics (MSCA 31012)
##### Date: 10/29/2021
##### Author: Jacqueline Pezan
##### Dataset: https://en.wikipedia.org/wiki/Iris_flower_data_set
##### Additional Resources: https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html

Your task is to optimize this model so it produces better predictions. A common technique is to do 'hyper parameter optimization.' Scikit-learn has methods built in to do this (see `GridSearchCV` and `RandomSearchCV`). However, in order to learn about loops, we will do this ourselves.

Try different values for the following parameters:
- criterion: 'entropy' and 'gini'
- max_depth: betwen 1 and 10
- min_samples_split: between 2 and 5

You are welcome to try optimizations beyond these values, but the list above is the minimunm required for this assignment.

Find the best set of parameters and have your program return them, along with the score.

If you reach accuracy of 1 (perfect prediction), stop searching and show the parameters.

You are expected to write a program to solve this optimization problem. You may not cust and paste the model training code for each test (that's A LOT of cutting and pasting). You may also not manually run the code many times where you manually try different values.

### Hints

You will need to train this model and score it multiple times (once for each set of parameters you are testing). Think in terms of loops (perhaps multiple nested loops).

You will also need to keep track of all three parameters and the score. Make sure you don't accidentally overwrite variables inside the loops.

Somehow, you will need to compare the current score with the best score you have achieved so far. If the current score is better than what you have already achieved, you should update the score, and the associated variables.

At the end of your program, print the best score and the associated variables.
