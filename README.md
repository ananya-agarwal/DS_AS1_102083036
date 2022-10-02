Time Series Prediction

Input: 9-day (Time Series) readings for 5 Parameters (Para9 to Para13)

Output: 10th-day readings for 5 Parameters (Para9 to Para13)

Model Used: Long Short Term Memory (LSTM)

Steps:
•	Data Preprocessing
•	Data Preparation
•	Model Selection and Training
•	Model Evaluation

Data Pre-processing:
•	Handling Null Values: Fill all the null values with 0
•	Removing incomplete data: Delete one instance having data for 9 days only

Data Preparation:
•	Rescaling all the parameter values using MinMax Scalar
•	Prepare the dataset in the input-output format for the model training
•	Split the dataset into training and testing sets (80-20 train-test split used)

Model Training:
•	Model Selection: LSTM has been used for training
•	Building the Model: Formation of LSTM layers and setting of different training parameters
•	Model Training: Feed the train set data to the LSTM model and train for 600 epochs

Model Evaluation:
•	Test the trained LSTM model on test set data by making predictions on test set data.
•	Rescale the values back to the original scale (Inverse Scaling) and compute root mean square error (RMSE) based on predicted and actual values
•	Visualize results by plotting graphs
After evaluation of the model on test set the observed RMSE value is 22.45 (approx).
 
