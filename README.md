#COMMENTS ON KFOLD MNIST Dataset Assignment

The aim of K-Fold Cross-Validation is assesing the performance of K-Nearest Neighbor on the MNIST dataset.
Splitting the data into numerous folds and training/testing the model on each fold ensures that the model's performance is not dependent on a train-test split. 
This gives a more generalizable model accuracy estimate.
The KFold object has 10 splits, dividing the data into 10 parts. The model is trained and tested 10 times, each time with a different fold as the test set and the rest as the training set. 
It helps get a complete performance metric.

ON OBSERVING THE RESULTS WE GET THE FOLLOWING

array([0.97171429, 0.97257143, 0.97057143, 0.97185714, 0.97071429, 0.97185714, 0.976, 0.97314286, 0.97157143, 0.97557143])


The KNN classifier works well on the MNIST dataset, with each fold's accuracy around 97%. 
The model's high accuracy shows it can recognise handwritten digits well. 
All 10 folds have accuracy scores between 0.9706 and 0.9760. 
This consistency suggests that the model performs similarly across data subsets.

When we compare the mean and standard deviation we get;

Mean accuracy: 97.255714%
Accuracy Standard Deviation: 0.176872%

According to these statistics, the model is reliable and robust due to its high accuracy and low variability.
