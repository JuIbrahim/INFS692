# Objective
The objective of this project is to develop different models to predict failure (endpoint) of the radiomics signature based from MRI, PET and CT scans.

# Data
The data used in this session is radiomics_completedata.csv. It has 197 observations and 498 variables. Failure.binary is the binary property to predict. The data is normalized before using in the model and is splitted into training set (80%) and testing set(20%).

# Model
In Model 1, we create an ensemle clasisfication model such as Bagging, SVM and GBM. We print the AUC values during training and testing set and also showed the top 20 important features during Training set. 
In Model 2, the deep learning (neural network-based classification model) is performed. In this model, we created five hidden layers with 256, 128, 128, 64 and 64 neurons, with respective activation functions of Sigmoid and is followed by a dropout to avoid overfitting. We also create an output layer with two neurons with respective activation functions of Softmax. We also did backpropagation compiler approach and trained the model with epoch = 10, batch size = 128 and validation split = 0.15. 
In Model 3, we compared the clustering techniques such as K-Means, Hierarchical and Model Based without considering the binary output and categorical variables.

