# Assignment: Unit 11 - Risky Business
 
### Submission

* The submission contains two notebooks (.ipynb) files named "Master_credit_risk_ensemble" and "Master_credit_risk_resampling-Trial".

* The resource data files (lending_data.csv and LoanStats_2019Q1.csv) have been uploaded in a folder named "Resources"

* The observations inlcuded in the notebooks are summarised below.

#### Resampling

Use the above to answer the following questions:

* Which model had the best balanced accuracy score?
> Compared to the original dataset's balanced accuracy score (BAS) of 0.954, all the remaining models had a very high BAS (greater than 0.99). Among the resampled data algorithms, the ClusterCentroids Model had a marginally lower score of 0.99328, while all the remaining had the same BAS of 0.99467.

* Which model had the best recall score?
> All models performed better than the original data set in terms of recall score. While the ClusterCentroids Model had a marginally lower recall (high risk: 0.99, low risk: 0.99, average: 0.99), other models had the same recall score (high risk: 1.00, low risk: 0.99, average: 0.99)

* Which model had the best geometric mean score?
>  All algorithms and resmapling techniques fared similarly in terms of geometric mean score of 0.99

#### Ensemble Learning

Use the above to answer the following questions:

* Which model had the best balanced accuracy score?
> Both models have the same balanced accuracy score (BAS) of 0.787

* Which model had the best recall score?
> Easy Ensemble Classifier (EEC) model has a relatively higher recall score (High Risk: 0.91, Low Risk: 0.94, Total: 0:94)

* Which model had the best geometric mean score?
> The EEC model has a higher geometric mean score (High Risk: 0.93, Low Risk: 0.93, Total: 0:93)

* What are the top three features?
> The top three features were "total_rec_prncp", "total_rec_int" and "total_pymnt_inv"
- - -



