# Overview of the analysis

Using Machine Learning and Neural Networks for this project, I used the features in the dataset to create a binary classifier that will help to predict if the applicants that will be funded by a Charitable organization called Alphabet Soup will be successful. For this analysis we had a dataset containing various measures on 34,000 organizations that have been funded by Alphabet Soup. This project compromised of the following 3 steps:

* Preprocessing the data for the neural network
* Compile, Train and Evaluate the Model
* Optimizing the model

## Resources
* Data Source: charity_data.csv
* Software: Python 3.7.7, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

# Results
## Data Preprocessing
* The target variable that was considered for this model: IS_SUCCESSFUL columns.
*  Variable(s) were considered to be the features for this model: every columns except IS_SUCCESSFUL column which was dropped.
*  Variable(s) were neither targets nor features, and should be removed from the input data: EIN and NAME column

## Compiling, Training, and Evaluating the Model
* The number of neurons, layers, and activation functions I selected for my neural network model were:
* There were 2 hidden layers with 80 neurons on first layer and 30 neurons on second layer.
* There were also an output layer.
* The first and second hidden layers had relu activation functions, and the output layer had sigmoid.
* I wasn’t able to achieve 75% target model performance. The accuracy of my model was 74%.
![image](https://user-images.githubusercontent.com/31675832/154862966-e43f6090-b975-4b88-8ad5-8604e0db202b.png)



# Summary
Overall, by increasing the accuracy above 75% we are able to correctly classify each of the points in the test data 75% of the time. And, an applicant has a 80% chance of being successful if they have the following:

* The NAME of the applicant appears more than 5 times (they have applied more than 5 times)
* The type of APPLICATION is one of the following; T3, T4, T5, T6, T7, T8, T10, and T19
* The application has the following CLASSIFICATION; C1000, C2000, C3000, C1200, and C2100.

A good model to recommend is the Random Forest model because Random Forest is good for classification problems. Using this model produces a 78% accuracy.
