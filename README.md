# Neural_Network_Charity_Analysis
## Analysis of Alphabet Soup’s Charity Funding program

### Overview of the Statistical Analysis:

The purpose of this analysis is to help Alphabet Soup predict whether applicants will be successful in accomplishing their mission if they receive funding. The analysis is being done to help Alphabet Soup decide where to make investments.

The data used in the analysis is a csv file of 34,000 organization that have received funding from Alphabet Soup in the past.  The dataset contains several datapoints in columns about each organization.

### Results: 

Data Preprocessing:
-	What variable(s) are considered the target(s) for your model?

The variable considered the target is the “IS SUCCESSFUL” column in the dataset.

-	What variable(s) are considered to be the features for your model?

The variables considered to be features are:
APPLICATION_TYPE – Alphabet Soup application type
AFFILIATION – Affiliated sector of industry
CLASSIFICATION – Government organization classification
USE_CASE – Use case for funding
ORGANIZATION – Organization type
STATUS – Active status
INCOME_AMT – Income classification
SPECIAL_CONSIDERATIONS – Special consideration for application
ASK_AMT – Funding amount requested

![DatasetFeatures](https://user-images.githubusercontent.com/99366022/178117239-3706e3e6-599c-47ae-ae1f-a172ee2214b7.png)

-	What variable(s) are neither targets nor features, and should be removed from the input data?

The variables that were removed from the input data are the “EIN” and “Name” identification columns as these datapoint didn’t enhance the outcome.
 
![EINnNameDrop](https://user-images.githubusercontent.com/99366022/178117248-aea303b5-5082-498c-b0f9-4fd65d124991.png)

Compiling, Training, and Evaluating the Model:
-	How many neurons, layers, and activation functions did you select for your neural network model, and why?

There were two hidden layers used in the model.  The first hidden layer had 80 neurons and the second hidden layer had 30 neurons.  The activation function for both the hidden layers was relu, with sigmoid used for the output.
 
![1st Model](https://user-images.githubusercontent.com/99366022/178117255-dbe8ae43-aaed-41eb-b1a1-843cc468f648.png)

-	Were you able to achieve the target model performance?

No, the model had an accuracy rate of 72.8%, which did not reach the 75% accuracy target.
 
![1st ModelAccuracy](https://user-images.githubusercontent.com/99366022/178117258-7f4352d5-7420-43e8-8cc6-6afa4004bbfc.png)

-	What steps did you take to try and increase model performance?

I tried to increase the models accuracy by adding more hidden layers, altering the number of neurons in each of the layers, as well as changing the activation method used in the layers.  This is the third attempt to optimize the model.
 
 ![3rdOptimizationModel](https://user-images.githubusercontent.com/99366022/178117268-c5a456e9-35f5-444e-a23b-d47b2aceda8f.png)

![3rdOptimizationModelAccuracy](https://user-images.githubusercontent.com/99366022/178117271-808ba822-5c50-43b9-a0d5-7bc1b0a66865.png)

### Summary:

The original mode had an accuracy of 72.8%.  I tried to increase the accuracy by optimizing the model and the results of the first attempt is 72.6%, the second attempt is 72.7% and the third attempt is 72.7%.  It seems that adding hidden layers, neurons, and changing the activation method didn’t increase the accuracy and barely moved it at all.  I’d recommend staying with the first model as it has the highest accuracy rate after 15 epochs.
