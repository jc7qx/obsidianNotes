XGBoost is an open source library providing a high-performance implementation of gradient boosted decision trees. An underlying C++ codebase combined with a Python interface sitting on top makes for an extremely powerful yet easy to implement package.

Boosting takes a more _iterative_ approach and is still technically an ensemble technique in that many models are combined together to perform the final one, but takes a more clever approach.

Rather than training all of the models in isolation of one another, boosting trains models in succession, with each new model being trained to correct the errors made by the previous ones. Models are added sequentially until no further improvements can be made. The advantage of this iterative approach is that the new models being added are focused on correcting the mistakes which were caused by other models. **Gradient Boosting** specifically is an approach where new models are trained to predict the residuals (i.e errors) of prior models.
---
title: Security in Intelligent Transport Systems for Smart Cities: From Theory to Practice
authors: Muhammad Awais Javed, Wassim Znaidi
year: 2016
---


install the library
```unix
pip install xgboost
```
setup dataset
set train-test split
transform data to DMatrix
```python
xgb.DMatrix(train data, label)
```
define xgboost paramters
```
eta, max_depth, objective, num_class
steps
```
training model
```python
model = sgb.train(param, D_train, steps)
```
testing model
```python
import_ numpy _as_ np  
from_ sklearn.metrics _import_ precision_score, recall_score, accuracy_score  
  
preds = model.predict(D_test)  
best_preds = np.asarray([np.argmax(line) _for_ line _in_ preds])  
  
print("Precision = {}".format(precision_score(Y_test, best_preds, average='macro')))  
print("Recall = {}".format(recall_score(Y_test, best_preds, average='macro')))  
print("Accuracy = {}".format(accuracy_score(Y_test, best_preds)))
```
hyperparameters tuning with scikit learn

x
```python
#run gridsearchCV
from_ sklearn.model_selection _import_ GridSearchCV  
  
clf = xgb.XGBClassifier()  
parameters = {  
	"eta" : [0.05, 0.10, 0.15, 0.20, 0.25, 0.30 ] ,  
	"max_depth" : [ 3, 4, 5, 6, 8, 10, 12, 15],  
	"min_child_weight" : [ 1, 3, 5, 7 ],  
	"gamma" : [ 0.0, 0.1, 0.2 , 0.3, 0.4 ],  
	"colsample_bytree" : [ 0.3, 0.4, 0.5 , 0.7 ]  
}  
  
grid = GridSearchCV(clf,  
	parameters, n_jobs=4,  
	scoring="neg_log_loss",  
	cv=3)  
  
grid.fit(X_train, Y_train)
```



