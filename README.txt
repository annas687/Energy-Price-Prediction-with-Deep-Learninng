# Energy Usage Prediction
Forecasting energy demand is critical for energy businesses and government agencies to hedge their assets and effectively ensure resource sustainability and availability. For energy forecasting, four distinct machine models are used: i) LightGBM (LGBM); ii) Recurrent Neural Network (RNN) ; iii) GRU Network; iv) Long short-term memory (LSTM)

The input elements are external environmental data, day//hour-type, and net energy consumption of various load types. The output represents the total energy consumption of the building's power utilisation. Based on raw data, modelling assessments for future energy use are carried out.

## Tech stack
> Warning: Python packages required to run the notebook.
### Required Libraaris
 * plotly, numpy,  seaborn, matplotlib (Data Visulasation)
 * datetime (Data Processing)
 * pandas, sklearn, LightGBM, bayesian_optimization, graphviz, pydot, json, tensorflow, tensorboard, statsmodels, hyperopt, keras, statsmodels(Machine Learning)
 
### Data Acquisition
The dataset was used for the development of the machine learning models, was taken from: https://www.kaggle.com/c/ashrae-energy-prediction/overview

  * `train.csv` - historic meter reading data by timestamp for the building
  * `weather_[train/test].csv` - historical weather data and weather forecast for one or a few places geographically close to the building
  * `building_metadata.csv` - metadata about the building, e.g., whether it is an office space, a restaurant, etc. 
  * `test.csv` - the meter, building id and timestamp we will be predicting for
  * `sample_submission.csv` - all the future data we would like to predict



## Documentation

  * `groupReport_G18.pdf` - final group report
  * `Ml_CW_Final_G18.jpynb` - Complete code with all the EDA + PRE-PROCESSING + MODEL IMPLEMENTATION
  * 'Readme' - Instructions and information related to the code and submission
  



Project
├── groupReport_G18.pdf
├── README.md
├── Ml_CW_Final_G18.jpynb
└── Logs
         ├── rnn_logs.zip
         ├── lstm_logs.zip
         └── gru_logs.zip
```


## How to Run code
The code has been segmented due to how the tasks were assigned. However some code, in particular the models require that the pre-processing code has been run first or that there is correct pre-processed data. As the datasets are rather large and a lot of pre processing is done we found some of these codes impossible to run on collab or any other virtual engine and so had to run it locally.
  * `Ml_CW_Final_G18.jpynb` - Can be run as long as the required impports are there, dataset is completely downloaded, paths are set properly and required libraries are installed. 
  * 'log zips' - All the logs from the trials that ran are in zip files with the filenames as per their respective model. 

## Tenssorboard 
To display the logs on tensorboard, it is recommended that it is run on Google colab, with the logs uploaded on google drive first. The reason for this is purely because running tensorboard was giving us path errors, which google colab eliminates. 


# Important Note
Dataset is extremely large and it is recommended that computing resources used to run the code, specially T3 part, has atleast 16GB of RAM and a cpu with more than 4 cores and newwer architecture.
