Gesture Phase Detection using classification algorithms##

The dataset is publicly available in the UCI Machine Learning Repository. The dataset is designed for studying Gesture Phase Segmentation and consists of features extracted from 7 videos capturing individuals performing gestures. Each video in the dataset is associated with two files. The first file is the raw file, which contains the positional information of the hands, wrists, head, and spine of the user in each frame of the video. The second file is the processed file, which includes the velocity and acceleration measurements of the hands and wrists. It has 9900 instances and 50 attributes.
Preprocessing##

Missing values are frequently encountered when working with real-world problem. In this dataset most of the numerical attributes are normally distributed hence missing values are filled with mean imputation. Phase is the target column. It has five classes, Label encoding is a method commonly employed in machine learning and data analysis to transform categorical variables into a numerical representation as many machine learning models works for only numeric data.Label encoding is done for converting phase catogorical into numerical. LDA is specifically designed for classification tasks and aims to find linear combinations of features that maximize the separation between classes. This dataset contains 50 attributes, Linear discriminant analysis reduction was used to reduce the number of attributes.

image
Model Evaluation###

The study was performed involving tuning the hyperparameters of the Gradient Boosting Classifier, Light GBM and KNN algorithms using Optuna. Bayesian optimization is performed using Optuna's create_study and optimize functions. The objective function is maximized to find the best set of hyperparameters for the Gradient Boosting classifier.
