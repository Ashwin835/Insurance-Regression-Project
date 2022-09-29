# Insurance Regression Project
 The dataset used for this project was obtained from the text "Machine Learning with R", by Brett Lantz. All code for this project was written solely by Ashwin Verma


# Project Description
The cost of insurance is determined by various factors such as region and sex. Using a dataset with various independent variables and an insurance price based on these variables, we want to find out which model will help in giving us the most accurate insurance price predictions. Finding the best fitting model has many factors to it, but for this project only the adjusted r^2 is being looked at, along with any major overfitting/underfitting. Some of the models tested are multiple linear 
regression, polynomial regression, support vector regression, decision tree regression, and random forest regression.




# Project Results 
                                                            MULTIPLE LINEAR REGRESSION 
This model had an adjusted r^2 of less than 80% on both the x test and trained data, making it not the best model to use.
Since the adjusted r^2 was less than 80%, we can conclude that slight underfitting also took place


                                                           POLYNOMIAL LINEAR REGRESSION 
 This model is better than multiple linear regression, however, the polynomial feature degree should be less than 5 to 
 avoid major overfitting. Polynomial feature degree 3 is the best in giving the most accurate predictive model.
#it predicts around 85% of the x train and test data correctly. Although this model is good, a better model is needed


                                                           SUPPORT VECTOR REGRESSION 
This model had an adjusted r^2 of 88% on the x trained and test data, making it a very solid model to predict prices.
 The algorithm for SVM effectively uses the support vector points, to alter in making a great model when compared with 
 multiple linear regression's adjusted r^2


                                                          DECISION TREE REGRESSION 
The decison tree model is by far the worst model to predict insurance prices. The algorithm split up the data up into n 
 trees, takes the average with the data from each tree, and so all predictive points in the range of each tree will be that
average value. This wasn't very good accurate algorithm given the dataset, as  the adjusted r^2 was only 72%, also showing that
 underfitting must have occured as well


                                                         RANDOM FOREST REGRESSION
Just like SVM, Random Forest Regression has a really good adjusted r^2, with both the trained and test x data being around 87%
 with 100 trees. The number of trees after 100, don't change the adjusted r^2 value much, but will eventually have the trained 
 x_data at a higher r^2 than the test data, showing a bit of overfitting 


                                                         BEST MODEL 
 Based on all the results, the best models to use in order to make accurate insurnace prices is the random forest regression
 and Support Vector Regression. Their adjusted r^2 were the highest, and both their algorithms helped in making
 the best predictive model, along with very little fitting bias
