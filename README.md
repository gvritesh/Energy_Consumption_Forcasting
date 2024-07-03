# Energy_Consumption_Forcasting
Here, I have used the opensource energy dataset available in the UCI Library containing 19735 rows and 29 columns. The data is collected every 10 minutes for energy usage and appliance usage based on different parameters like temperature , humidity at each room along with some outside parameters like outside temperature, windspeed,dewpoint and visibility.
We are making a model architecture using stacked LSTM( Long Short Term Memory) to do an multivariate time series forcasting in the appliance usage column.
First we detect the outliers and use the min max scaler to scale the data so that the convergence of gradients become faster.
Then we call the TimeseriesGenerator function and then train test split the data.
Then we form the model architecture using Stacked LSTMs along with LeakyReLU as activation function and dropuout layers in between.
Then we compile the data using mean squared error with adam optimiser and metrics is set as mean absolute error.
Finally we make the prediction and plot the actual and predicted usage value using matplotlib.
