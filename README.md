# Deep-Learning-Challenge

## Background

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

### Step 1: Preprocess the Data

1. Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your dataset:
* What variable(s) are the target(s) for your model?
* What variable(s) are the feature(s) for your model?

2. Drop the EIN and NAME columns.

![Drop](/Images/drop_EIN_and_name.png)

3. Determine the number of unique values for each column.

![Unique](/Images/determine_unique_value.png)

4. For columns that have more than 10 unique values, determine the number of data points for each unique value.

5. Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, Other, and then check if the binning was successful.

6. Use pd.get_dummies() to encode categorical variables.

![Dummies](/Images/get_dummies.png)

7. Split the preprocessed data into a features array, X, and a target array, y. Use these arrays and the train_test_split function to split the data into training and testing datasets.

8. Scale the training and testing features datasets by creating a StandardScaler instance, fitting it to the training data, then using the transform function.

### Step 2: Compile, Train, and Evaluate the Model

1. Continue using the file in Google Colab in which you performed the preprocessing steps from Step 1.

2. Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.

3. Create the first hidden layer and choose an appropriate activation function.

4. If necessary, add a second hidden layer with an appropriate activation function.

5. Create an output layer with an appropriate activation function.

6. Check the structure of the model.

7. Compile and train the model.

8. Create a callback that saves the model's weights every five epochs.

9. Evaluate the model using the test data to determine the loss and accuracy.

![Results 1](/Images/Results_1.png)

10. Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity.h5.

[Model 1](/Models/AlphabetSoupCharity1.h5)


### Step 3: Optimize the Model

Using your knowledge of TensorFlow, optimize your model to achieve a target predictive accuracy higher than 75%.

Use any or all of the following methods to optimize your model:

* Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:
    * Dropping more or fewer columns.
    * Creating more bins for rare occurrences in columns.
    * Increasing or decreasing the number of values for each bin.
    * Add more neurons to a hidden layer.
    * Add more hidden layers.
    * Use different activation functions for the hidden layers.
    * Add or reduce the number of epochs to the training regimen.

Note: If you make at least three attempts at optimizing your model, you will not lose points if your model does not achieve target performance.

1. Create a new Google Colab file and name it AlphabetSoupCharity_Optimization.ipynb.

2. Import your dependencies and read in the charity_data.csv to a Pandas DataFrame.

3. Preprocess the dataset as you did in Step 1. Be sure to adjust for any modifications that came out of optimizing the model.

4. Design a neural network model, and be sure to adjust for modifications that will optimize the model to achieve higher than 75% accuracy.

![Results 2](/Images/Resuts_2.png)

![Results 3](/Images/Results_3.png)

5. Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity_Optimization.h5.

[Model 2](/Models/AlphabetSoupCharity2.h5)

[Model 3](/Models/AlphabetSoupCharity3.h5)

### Step 4: Write a Report on the Neural Network Model

For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for Alphabet Soup.

The report should contain the following:

1. Overview of the analysis: Explain the purpose of this analysis.

2. Results: Using bulleted lists and images to support your answers, address the following questions:

* Data Preprocessing

    * What variable(s) are the target(s) for your model?
    * What variable(s) are the features for your model?
    * What variable(s) should be removed from the input data because they are neither targets nor features?

* Compiling, Training, and Evaluating the Model

    * How many neurons, layers, and activation functions did you select for your neural network model, and why?
    * Were you able to achieve the target model performance?
    * What steps did you take in your attempts to increase model performance?

* Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

[Report](/Deep_Learning_Challenge_Report.pdf)

### Step 5: Copy Files Into Your Repository

Now that you're finished with your analysis in Google Colab, you need to get your files into your repository for final submission.

1. Download your Colab notebooks to your computer.

2. Move them into your Deep Learning Challenge directory in your local repository.

3. Push the added files to GitHub.


## References

* [IRS. Tax Exempt Organization Search Bulk Data Downloads.](https://www.irs.gov/Links)
* [Neptune.Ai](https://neptune.ai/blog/google-colab-dealing-with-files)
* [Write and Save Files in Python](https://colab.research.google.com/github/computationalcore/introduction-to-python/blob/master/notebooks/4-files/PY0101EN-4-2-WriteFile.ipynb#scrollTo=43rIWbQI0up-)
