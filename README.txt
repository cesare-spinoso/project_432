README for G16
--------------
Our project relies mainly on numpy, pandas, sklearn, statsmodels and PyTorch.
Our code submission contains the following files:
	./Data/ <-- raw data set for electricity and weather data
	./IesoMerged.csv <-- Merged electricity dataset
	./MergedDataset.csv <-- Merged electricity and weather dataset with outliers handled.
	./Electricity.ipynb <-- notebook for extracting our data
	./Outliers.ipynb <-- notebook for preprocessing and handling outliers
	./Timeseries_Analysis.ipynb <-- notebook for time series forecasting methods
	./Linear_models.ipynb <-- notebook for linear model related models and methods
	./Neural_networks.ipynb <-- notebook for neural network related models
	./Final_results.ipynb <-- notebook for our final (test set) prediction and metrics
	./best_design_matrix.csv <-- The output from Linear Models to be used for the Final Results notebook
	./output_* <-- all of the related outputs (log runs and plots) for each corresponding notebook (time series, linear models, neural networks and final results).

* The files should be run in the order:
  Electricity.ipynb
  Outliers.ipynb
  Timeseries_Analysis.ipynb
  Linear_models.ipynb (colab)
  Neural_networks.ipynb (colab)
  Final_results.ipynb 
  Note: You can run Linear_models.ipynb and Neural_networks.ipynb concurrently. Once Linear_models.ipynb finishes running, you can start running Final_results.ipynb since it relies on the results from Linear_models.ipynb.
* GPU is required for the autoencoder training in Linear_models.ipynb and for all of the Neural_networks.ipynb (Google colab was used for this)
	Linear models colab link: https://colab.research.google.com/drive/1TxfXvyPbPnFwwasUPalzfyrPCCGTI1rL?usp=sharing
	Neural network colab link: https://colab.research.google.com/drive/1Eg9w7knWacjDc4cUDYNFJfNY8mxT-SXf?usp=sharing
	(MergedDataset.csv must be uploaded for this to work.)
* Training takes ~30 min for the Timeseries_Analysis.ipynb, ~12 hours for Linear_models.ipynb and ~24 hours for the Neural_networks.ipynb.
* For the autoencoder we relied on:
https://medium.com/@vaibhaw.vipul/building-autoencoder-in-pytorch-34052d1d280c
* For the LSTM and GRU training we relied on:
https://stackabuse.com/time-series-prediction-using-lstm-with-pytorch-in-python/
https://www.jessicayung.com/lstms-for-time-series-in-pytorch/

The electricity data was downloaded from https://www.ieso.ca/en/Power-Data/Data-Directory.
The weather data was downloaded from https://www.renewables.ninja/.