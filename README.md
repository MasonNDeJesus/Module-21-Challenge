# Module-21-Challenge
Repository for the Neural Networks and Deep Learning Module

Starter_Code_21 Folder:
- Neural_Network_Deep_Learning_Final_Code file
- AlphabetSoupCharity.h5 file
- Results and Analysis Report.docx file (Didn't know if this needed to be in a word document or the readme so I'll do both)

Results
Data Preprocessing:
-	Target Variable:
  -	The target variable for the model is “IS SUCCESSFUL”, which indicates whether the funding was used effectively (1) or not (0).
-	Feature Variables:
  -	The features for the model include:
    -	APPLICATION_TYPE
    -	AFFILIATION
    -	CLASSIFICATION
    -	USE_CASE
    -	ORGANIZATION
    -	STATUS
    -	INCOME_AMT
    -	SPECIAL_CONSIDERATIONS
    -	ASK_AMT
-	Variables to be Removed:
  -	The following columns were removed from the input data as they are neither targets nor features:
    -	EIN
    - NAME
Compiling, Training, and Evaluating the Model
-	Neurons, Layers, and Activation Functions:
  -	The model consists of:
    -	Input layer with 43 input features.
    -	Two hidden layers, each with 30 neurons and using the ReLU (Rectified Linear Unit) activation function to introduce non-linearity.
    -	An output layer with a single neuron and a Sigmoid activation function for binary classification.
-	Achieved Performance:
  -	The model achieved an accuracy of approximately 72.91% on the test dataset, with a loss of 0.5631.
-	Steps Taken to Increase Model Performance:
  -	Adjusted the number of neurons and layers in the network.
  -	Experimented with different activation functions.
  -	Scaled the input features using “StandardScaler” to ensure that all features contribute equally to the model’s performance.

Summary

The deep learning model developed for the Alphabet Soup project shows promising results with a classification accuracy of 72.91%. While the model does not perform above 75% yet, the steps taken for optimization could potentially improve performance further.

Recommendation for Alternative Models

To improve classification performance, I recommend exploring ensemble methods such as Random Forest or Gradient Boosting. They can capture complex interactions between features and may outperform a single neural network, particularly with tabular data. They also offer greater interpretability, which can be valuable for stakeholders in understanding the decision-making process behind funding approvals. To note: Random Forest builds multiple independent trees and aggregates the predictions. Gradient Boosting builds the trees sequentially, with each one learning from the previous.
