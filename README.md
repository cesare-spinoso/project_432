# Predicting electricity demand in the Greater Toronto Area
This project uses time series forecasting, linear models and neural networks in an attempt to accurately predict the hourly electricity demand of the Greater Toronto Area (GTA) for a period of half a year.

Our project relies mainly on numpy, pandas, sklearn, statsmodels and PyTorch.

# How to navigate the files
./Data/ <-- raw data set for electricity and weather data
./IesoMerged.csv <-- Merged electricity dataset
./MergedDataset.csv <-- Merged electricity and weather dataset with outliers handled.
./Electricity.ipynb <-- Notebook for extracting our data
./Outliers.ipynb <-- Notebook for preprocessing and handling outliers
./Timeseries_Analysis.ipynb <-- Notebook for time series forecasting methods
./Linear_models.ipynb <-- Notebook for linear model related models and methods
./Neural_networks.ipynb <-- Notebook for neural network related models
./Final_results.ipynb <-- Notebook for our final (test set) prediction and metrics
./best_design_matrix.csv <-- The output from Linear Models to be used for the Final Results notebook
./output_* <-- All of the related outputs (log runs and plots) for each corresponding notebook (time series, linear models, neural networks and final results).

The files should be run in the order:
<ol>
  <li>Electricity.ipynb</li>
  <li>Outliers.ipynb</li>
  <li>Timeseries_Analysis.ipynb</li>
  <li>Linear_models.ipynb (colab)</li>
  <li>Neural_networks.ipynb (colab)</li>
  <li>Final_results.ipynb</li>
</ol>
Note: You can run Linear_models.ipynb and Neural_networks.ipynb concurrently. Once Linear_models.ipynb finishes running, you can start running Final_results.ipynb since it relies on the results from Linear_models.ipynb.

You can also access some of the notebooks on Google Colab
<ul>
	<li>Linear models colab link: https://colab.research.google.com/drive/1TxfXvyPbPnFwwasUPalzfyrPCCGTI1rL?usp=sharing</li>
	<li>Neural network colab link: https://colab.research.google.com/drive/1Eg9w7knWacjDc4cUDYNFJfNY8mxT-SXf?usp=sharing</li>
</ul>

## External resources
For the autoencoder we relied on:
https://medium.com/@vaibhaw.vipul/building-autoencoder-in-pytorch-34052d1d280c
For the LSTM and GRU training we relied on:
https://stackabuse.com/time-series-prediction-using-lstm-with-pytorch-in-python/
https://www.jessicayung.com/lstms-for-time-series-in-pytorch/

The electricity data was downloaded from https://www.ieso.ca/en/Power-Data/Data-Directory.
The weather data was downloaded from https://www.renewables.ninja/.

# Results
Our goals, methodology and results are explained in full in the provided report.
