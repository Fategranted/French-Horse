# French-Horse
Group Project for CANSSI Competition

We are using a neural network to predict the probability. Our model is in the google colab.

If you want to train the model from start, you could use this colab:
https://colab.research.google.com/drive/1MlxxjwTKnLSINT7mIBwXjZvbDdyHkl37?usp=sharing \
Instruction for this colab: 
1. Upload your csv training data to the colab and rename it to "training_data.csv". 
2. Upload the csv data you want to predict and rename it to "custom_data.csv". 
3. Run the code from the start.
   
Notes and warnings: 
 - You can change the number of epochs in the training process, but it may take very long time to train when your training data is big. 
 - The column names may vary if you upload csv files in the different format from we originally did. This may cause errors when processing the data. \
   The things we do in processing the data is drop all the non-numeric columns, drop all rows have nans, and convert all numeric values to type float.
   
Predicted Results:
 - The last dataframe named "predicted_result" contains the horse_id, race_id, and the predicted win_probability. 
 - We also export the predicted result in a csv file named "predicted_result.csv".
