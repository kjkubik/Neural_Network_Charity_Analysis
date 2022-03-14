# Neural_Network_Charity_Analysis

### Purpose: 
Alphabet Soup wants to know when their donations to charities will be most successful.  By creating a binary classifier we are hoping to be able to help Alphabet Soup know exactly what works and what doesn't work in the world of Charity.

### Proceedure: 
The first thing needing to be accomplished was the preprocessing of the data for our deep neural network model.
To do so, we: 
    - determined columns that were features, targets and 'throw-aways'
    - removed the 'throw-away columns
    - checked the number of unique values left for each column 
![](images/unique_values_for_original_columns.png)
   
   - get application type and classification columns bucketed
![](application_type_buckets.png)

![](classification_buckets.png)

    - generate the categorical variable list
![](categorical_variable_list.png)
    
    - encoding with OneHotEncoder
    
    - replace the original columns with OneHotEncoders encoded features
    
    - train, fit/test and scale the data
    
Next, we compile, train and evaluate the deep neural network model. Here's the summary of the model setup: 
![](Summary.png)

After that, we compile and after evaluating the module we can see it is not performing very well:

![](Evaluation_of_Nueral_Network.png)

So, we decide to attempt working with TensorFlow to optimize my model in order to achieve a target predictive accuracy higher than 75%. 

The following was attempted to optimize my model to achieve a higher target predictive accuracy:

- Adjusting the input data to ensure that there are no variables or outliers that are causing confusion in the model, such as:
- Dropping more or fewer columns.
- Creating more bins for rare occurrences in columns.
- Increasing or decreasing the number of values for each bin.
- Adding more neurons to a hidden layer.
- Adding more hidden layers.
- Using different activation functions for the hidden layers.
- Adding or reducing the number of epochs to the training regimen.
    


### Results: 

- Deliverable 3: Optimize the Model
- Deliverable 4: A Written Report on the Neural Network Model (README.md)
