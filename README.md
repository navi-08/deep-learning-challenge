# deep-learning-challenge
deep learning challenge


The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special considerations for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively


The report should contain the following:

Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists and images to support your answers, address the following questions:

Data Preprocessing

What variable(s) are the target(s) for your model?
The target variable is the 'IS_SUCCESSFUL' column from application_df

What variable(s) are the features for your model?
The feature variables are every other column from application_df --> this was defined by dropping the 'IS_SUCCESSFUL' column from the original dataframe

What variable(s) should be removed from the input data because they are neither targets nor features?
Both 'EIN' and 'NAME' columns were dropped/removed, because they were neither targets nor features for the dataset.




Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
In the first attempt, i used 80 hidden_nodes_layer1 and 30 hidden_nodes_layer2  and 1 neuron ,utilizing ReLU activation functions for each layer



QUE. Were you able to achieve the target model performance?
ANS. -I was not able to achieve the 75% model accuracy target. An accuracy of approximately 72.43% and a loss of around 1.1584 on the test data, it's essential to compare these metrics against predefined performance goals or benchmarks to determine whether the model meets the desired criteria

 QUE. What steps did you take in your attempts to increase model performance?
ANS. I added more layers, removed more columns, added additional hidden nodes, and switched up the activation functions associated with each layer in an attempt to achieve higher model accuracy.



evaluation results

Model Evaluation Report

The model was evaluated on a test dataset to assess its performance. The evaluation yielded the following results:

- Loss: 1.1584
- Accuracy: 72.43%

These metrics provide insights into the model's effectiveness in predicting the ethnicity of individuals. The loss value indicates the discrepancy between the true ethnicity labels and the predictions made by the model. In this case, a lower loss value signifies better alignment between the predicted and actual labels.

The accuracy metric reveals the proportion of correctly classified instances, specifically indicating that approximately 72.43% of individuals' ethnicities were accurately predicted by the model. This suggests a moderate level of accuracy in identifying individuals as Indian based on the provided features.

It's important to note that while the model demonstrates some success in classifying individuals' ethnicities, further refinement and validation may be necessary to enhance its predictive capabilities.


Summary:

It seems like you are training a neural network model over 250 epochs, and you're displaying the loss and accuracy metrics for each epoch. The model appears to be making good progress as the loss decreases and accuracy increases over the epochs. Here's a summary of what's happening:

- Loss: The loss is decreasing steadily, indicating that the model is learning and improving its predictions over time.
- Accuracy: The accuracy is increasing, which means the model's predictions are becoming more accurate as training progresses.

It's essential to monitor these metrics to ensure that the model is learning correctly and not overfitting or underfitting the data. Additionally, you might want to visualize these metrics using plots to gain deeper insights into the training process.
