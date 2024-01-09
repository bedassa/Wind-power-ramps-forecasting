# Enhancing Wind-Power-Ramps-Forecasting

![Badge](https://img.shields.io/badge/Enhancing-forecsting-informational) 




Neural network is useful to capture the nono-linear relationship between input and output data. In this script, I use different architecture of neural network to generate wind power production for the Belgian wind farm fleets by using the climate output ERA5 and GFS data. The wind speed and other meteorological parameters are obtained from ERA5 and GFS. Prior to use the neural network to generate the forecast, some of the preprocesses steps hat have been used are:

- Spatial correlation between wind power and gridded climate data
+ Check data imbalance between training and validation which is very common in classiication but a little not straightforward in numerical data
* Take precautions in data splitting to avoid data leakage of temporal data
* consider benchmark model, for instance empirical convert wind speed into wind power using power curve

# Source of data
All the datasets are available in public domain. The links are:

- Wind power generation: https://www.elia.be/en/grid-data/power-generation/wind-power-generation
+ ERA5: https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels?tab=form
* GFS: https://www.ncei.noaa.gov/products/weather-climate-models/global-forecast


# Model development 
 MLP_GFS and MLP_ERA5 use the ERA5 and GFS input data, respectively to model wind power for the belgian offshore wind power. Before writing the model architecture it is important to prepare data and load all necessary pacakges. Once all the pacakges and data are ready, begin with simple architecture of the model, and then try to add more layers to see how is the performance of the model will be improved. Also, Look into the learning curve of training and validation curve since it provides valuable informtion either the model is overfittining, optimum or underfitting. 
 
  
