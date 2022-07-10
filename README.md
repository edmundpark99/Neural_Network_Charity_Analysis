# Neural_Network_Charity_Analysis

**Overview**

The main purpose of this analysis was to utilize machine learning alongside neural networks to create a binary classifier that can predict whether applicants will be successful if they apply to a given program, in this case, Alphabet Soup. We utilized a dataset with nearly 34,000 applicant organizations funded by this program and performed a neural network analysis to analyze the data.

**Results**

*Data Preprocessing*

- Our target variable for this model is "IS_SUCCESSFUL"
- Our feature variables for this model are "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT"
- "EIN" and "NAME" are neither targets nor features and were dropped.

*Compiling, Training, and Evaluating the Model*

![Learning Model](https://user-images.githubusercontent.com/6594718/178161530-dd8a88ae-c5d7-48db-a621-08ba138a2ce1.png)

- We had two hidden layers, with the first having 80 neurons and the second having 30 neurons. We had three activation functions, two reLu functions for the hidden layers and a sigmoid function for the output layer. 

![Accuracy](https://user-images.githubusercontent.com/6594718/178161696-6e98142c-3d83-48a0-8c77-f742c44cf77e.png)

- We were not able to achieve the desired target performance of 75%. The model only had an accuracy of 73.1%, just missing out on the desired target performance.

![Neuron Addition](https://user-images.githubusercontent.com/6594718/178161804-5a23352e-604a-44b9-9d69-50af41a3f99b.png)
![Third Hidden Layer](https://user-images.githubusercontent.com/6594718/178161830-826f9049-7db8-46bb-9d87-b78792f63b6b.png)
![Changing Activation Functions](https://user-images.githubusercontent.com/6594718/178161850-4c29fdec-9bac-4dd7-9408-976f97fe3d44.png)

- The main things I did to attempt to increase performance were adding more neurons to the hidden layers, adding a third hidden layer, and changing the activation functions for said hidden layers.

*Summary*

All in all, the results of the model were not able to achieve the target accuracy of 75%, both in the original attempt and in all three attempts to adjust the model. A good model that could be used in the future is the Random Forest Classifier in order to randomize the data and split it into smaller categories. Bucketing the data would also be useful in said model as well, even with the large dataset.
