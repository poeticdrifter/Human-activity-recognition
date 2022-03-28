# Human-activity-recognition
Dataset link: https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones
Machine learning models to recognize the activity of a person based on the activities carried out. Sensors were used to collect the data from different users while they were doing their regular works. Problem statement: Perform exploratory data analysis to check for: Build a machine learning model to classify the data Cluster the data using K-Means clustering algorithm. The value of K shouldn’t be based on the given class information. Instead, use elbow criteria to find the optimal value for K to cluster the data. Compare the results of both classification and clustering techniques. Check of there are any false negative, false positive cases.
Meta data regarding the dataset -
The Human Activity Recognition database was built from the recordings of 30 study participants performing activities of daily living (ADL) while carrying a waist-mounted smartphone with embedded inertial sensors. The objective is to classify activities into one of the six activities performed.

Description of experiment:-

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKINGUPSTAIRS, WALKINGDOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

Attribute information

For each record in the dataset the following is provided: 1.Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration. 2.Triaxial Angular velocity from the gyroscope. 3.A 561-feature vector with time and frequency domain variables. 4.Its activity label. 5.An identifier of the subject who carried out the experiment.
Models Implemented:
KNN	
Decision Tree	
Random forest	
SVM	


Reason why didn't use precision, recall and F1 score to compare our models are:-

Precision matters when there is high cost associated with false positives
Recall matters when there is high cost associated with false negatives
F1 score is better for imbalance classes
Since, Our problem statement is a multi class Classification problem, and not a binary classification so we cannot really identify false postives and false negatives. So our selection of model is based on the training and testing accuracy and the consistency of the model.

CONCLUSION-
Since there is a significant difference in the train and test accuracies of KNN and decision tree, these models become inconsistent.

And In Random Forest, test accurcay is more than the train accuracy which also makes it inconsistent.

So after going through all the evaluation metrics,  I come to a conclusion that SVM is the best fit model for our dataset.
