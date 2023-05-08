# Intro.-to-ML
We trained various linear regression models using only Voltage data and compared their
performace based on the Mean Absolute Error metric. We used Scikit-learn to prepare these models.

  Model                 MAE (O3)            MAE (NO2)       Remarks
Linear Regression   5.625937735514925 6.540100093842793   No regularization
Ridge               5.626671848882224 6.536821620242424   α = 1000
Lasso               5.625934686641408 6.537024370281168   α = 0.0001


Conclusion:While Ridge Regression best predicted the O3 values, Lasso performed better for N02 levels. Lasso 
performed better based on the combined MAE values.

We trained various linear and non-linear regression models using all available features
except the Timestamp and compared their performace based on the Mean Absolute Error metric.
Based on MAE scores, K Neighbours Regression performed best on the dummy_test.csv dataset.
 
       KNeighboursRegressor
     Hyperparameter      Value
      n_neighbours         1
      algorithm          kd_tree
      leaf_size           100
        metric          minkowski

Preparing Final model
Both Decision Tree Regressor (DTR) and K Neighbours Regressor (KNR) performed similarly
on the test data set. However since the KNR model had smalled disk size, we have submitted
KNeighboursRegressor as the final model. The model has a combined MAE of 0.0255472 over
dummy_test.csv dataset
