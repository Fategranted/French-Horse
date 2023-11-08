# French-Horse
Group Project for CANSSI Competition

The goal of this is to develop a model that can be used to predict the probability of a horse winning in a race. We will be using a neural network to make the prediction. We have developed our model in Google colab. 

The main idea of the model is to develop several layers each using linear regression and then using them to develop a prediction for the data. We then compute for the probability of each individual horse winning the race based on the finish position of each horse. 

If you want to train the model from start, you could use this colab:
https://colab.research.google.com/drive/1MlxxjwTKnLSINT7mIBwXjZvbDdyHkl37?usp=sharing 

Instruction for this colab: 
1. Upload your csv training and testing data to the colab and rename it to "training_data.csv" and "testing_data.csv". 
2. Upload the csv data you want to predict and rename it to "custom_data.csv". \
_You can also use the training and testing data we provide in the github repo. We also have a sample data for custom data_
3. Run the code from the start.
   
Notes and warnings: 
- You can change the number of epochs in the training process, but it may take very long time to train when your training data is big. 
- The column names may vary if you upload csv files in the different format from we originally did. This may cause errors when processing the data. 
- We also converted some non-numeric columns into numeric columns through defining each entry with a specific value. 
- When processing the data, we decided to drop all the non-numeric columns, drop all rows have nans, and convert all numeric values to type float.
   
Predicted Results:
- The last dataframe named "predicted_result" contains the horse_id, race_id, and the predicted win_probability. 
- We also export the predicted result in a csv file named "predicted_result.csv".


You can also try our trained model here:\
https://colab.research.google.com/drive/18tOyBDOzCOv-jWISi67R3mQxrZjJM2SH?usp=sharing

Instruction for this colab: 
1. Upload the trained model, "trot_model_state_dict.pth", that we provide in the github repo.
2. Upload the csv data you want to predict and rename it to "custom_data.csv". 
3. Run the code from the start.

Predicted Results:
- The last dataframe named "predicted_result" contains the horse_id, race_id, and the predicted win_probability. 
- We also export the predicted result in a csv file named "predicted_result.csv".
