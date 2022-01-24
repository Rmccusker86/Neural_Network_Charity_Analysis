# Neural_Network_Charity_Analysis

## Overview of the project
We were tasked with using Machine Learning and Neural Networks to create a binary classifier that would help predict if applicants could be funded by a charity organization. There was a dataset of over 34,000 different organizations. Given this info we were asked to do the following:
* Preprocess the Data
* Compile, Train, and Evaluate the Model
* Optimize said model in hopes of acheiving over 75% accuracy

# Results
## Pre-Processing the Data
* Varialbles to be considered as the target for the model: IS_SUCCESSFUL
* The feature variables for the model were the following columns: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT. 
* The columns EIN and NAME were identified as information not useful for this particular model and were subsequently removed.

## Compiling, Training, and Evaluation the Model
For my intial neural network model there were two hiden layers, with 100 and 30 neurons respectively. Both layers were given the "relu" activation function as that was shown to be the most succesful one. The output layer was given the "sigmoid" function.
![image](https://user-images.githubusercontent.com/88358771/150717249-8944a92c-3522-4d0d-a2a3-cf5503e9c0c2.png)

The target performance for this project was 75%, unfortunately I was only able to get my model's accuracy up to 73% as shown below
![image](https://user-images.githubusercontent.com/88358771/150717365-9a439e99-e49c-4f82-b7c6-b62bbceafab7.png)

If the asked accuracy percentage was not reached, we were asked to take steps to try and increase the model's overall performance
With my second test, I added an additional hidden "relu" activated layer. The three hidden layers had 100, 50, and 15 neurons.
![image](https://user-images.githubusercontent.com/88358771/150717604-1bcf51f3-b134-437a-b7fa-36bf0e769fe7.png)

With these added steps I was not able to raise the accuracy level .001 percent which rounded to 73%
![image](https://user-images.githubusercontent.com/88358771/150717690-54e3cf27-9f52-4bde-9c3b-b4ca0927be71.png)

For the third test, I kept three hidden layers with neurons of 100, 40, and 15, but changed the activation function of the third to "tanh"
![image](https://user-images.githubusercontent.com/88358771/150717771-dfc919d6-cd43-45ec-9547-9cc3d3cfbc61.png)

These results almost mimicked the other two, being .001 lower than the original results.
![image](https://user-images.githubusercontent.com/88358771/150717831-27ffaac7-1eb5-4792-9ad7-2dbe4b27339c.png)

## Summary
This deep learning model was not able to reach the target of 75% accuracy. Although coming close at 73, I would say that this model is not performing at a level that would be needed in most applications. Suggestions or better options to achieve these results would possibly be trying to use a different machine learning model such as RandomForestClassifier since those generally are able to consistently perform at a higher level.
