# Energy_Consumption_forecasting_with_Deep_Learning
Forecasting energy consumption in the mid and long-term with LSTMs using TensorFlow2 and Keras

The data was obtained from Kaggle. The dataset consists of 'Date' in the YYYY-MM-DD HH:MM:SS format and hourly energy production in megawatt('AEP_MW'). No missing values were found. 

The next step was Feature Extraction, reformatted the datetime column and extracted the year, month, date, day, week and time individually. 
We also plotted the yearly energy consumption to visually check for trends and seasonality. 

The dataset contains over 120,000 datapoints. So instead of having hourly values, we resampled the data in such a way we only have one value per day. We considered only the average value per day. 
We then split the dataset into test and training set and implemented the machine learning model to pattern predict future values. 
