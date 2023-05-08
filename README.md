# Intro.-to-ML
We trained various linear regression models using only Voltage data and compared their
performace based on the Mean Absolute Error metric. We used Scikit-learn to prepare these models.

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
