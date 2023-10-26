# PWC_Internship 

#The first task in this internship is to analyse the dataset provided and build classification model.
#The dataset contains features which can detect if the customer will subscribe to the product that the bank agent advised over the phone or not.
#On analysing it can be found that the target variable has more counts of 'No' compared to 'Yes' . It is imbalanced in the ratio of 90:10%.


#Insights drawn from scatter plot

##nr.employed has positive relation with emp.var rate, cons price idx, cons conf idx,
##eurobor has non-linear relation with emp.var rate, nr.employed. cons price & cons conf has same pattern observed( non linear relationship )
##consconf has similar non linear relation with emp.var rate & cons.conf.non linear relation with euribor & nr. employed
#consprice has linear (positive) with emp var rate, negative linear relationship with cons conf. non linear with nr.employed & eurobor
##emp var has positive linear with consprice & nr employes.Negative relationship with consconf.non linear with euribor
##duration & campaign follows similar pattern with all other variables(non linear)
##pdays follows similar non linear relationship with all other variables


#Model performance
DecisionTree        0.511816  0.722918  0.887572   0.507793  0.522414
LogisticRegression  0.517881  0.934369  0.911236   0.666717  0.423563
RandomForest        0.531541  0.938414  0.911722   0.667173  0.439368
Gradient Boosting   0.582778  0.946386  0.915801   0.659841  0.521839
XG Boost            0.579682  0.945734  0.912305   0.630299  0.536782
Best Model per Metric
F1: Gradient Boosting
Roc_auc: Gradient Boosting
Accuracy: Gradient Boosting
Precision: RandomForest
Recall: XG Boost
