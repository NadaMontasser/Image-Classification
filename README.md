# Image-Classification
Models used in this project:
1) KNN from Scracth
2) Logistic Regression
3)Support Vector Machine

##we had 10 models, one for each class on the train. The LR provides Accuracy of Predicted Class: 36.46%, also trained the model on 20000 samples and test on 10000 samples 


Part 3, first,  SVCLeaner() base model, which gave us a 23.5% accuracy.
•	Then we looked at the effect of C cost on SVC accuracy. We looked at the cost in [0.01, 0.1, 1, 10, 100] and found that the best accuracy is 36.5 with a cost of 0.0001, indicating that a low value of C will cause the model to look for a hyperplane with a larger margin of separation. The model will separate the model appropriately.
•	Then we applied the Regularization technique using Ridge L1 regressor with the cost to know its effect on the performance of the model, we discover that cost 1 with L1 gave us the highest accuracy 36.9%. L1 has a positive effect on the accuracy of the model that works on feature selection, which is useful in our case because we have a large number of images. L1 avoids features with zero coefficients.
•	Then, when building the SVC, we used the RBF kernel, which gave us 42.3% accuracy.
•	The Last tuning is the search for the best combination of Cost equal to 100 and gamma equal to 0.01 which gave us 44.6% accuracy 
