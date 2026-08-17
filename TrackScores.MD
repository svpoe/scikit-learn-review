CHANGE: Initial setup - Scaled logistic regression scored with 5-fold F1 on the training portion
CV F1 scores: [0.66666667 0.76923077 0.73170732 0.69565217 0.68421053]
Mean CV F1: 0.7094934906398879

CHANGE: stratify=y
CV F1 scores: [0.72222222 0.68181818 0.82926829 0.86363636 0.75555556]
Mean CV F1: 0.77050012318305

CHANGE: cross validation 
{'classifier__C': 0.1, 'classifier__solver': 'liblinear'}
0.7705860892264629

CHANGE: cross validation w/o stratified
{'classifier__C': 0.01, 'classifier__solver': 'liblinear'}
0.7189472845994586

CHANGE: Random forest w/ gridsearch
{'classifier__max_depth': None, 'classifier__min_samples_leaf': 5, 'classifier__n_estimators': 50}
0.890225916453538


FINAL EVAL WITH RANDOM FOREST
Accuracy: 0.9
Precision: 0.8387096774193549
Recall: 0.896551724137931
F1: 0.8666666666666667

Confusion matrix:
[[46  5]
[ 3 26]]

        PREDICTED
 ACTUAL [[TN FP]
        [ FN TP]]