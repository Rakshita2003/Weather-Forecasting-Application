# Weather-Forecasting-Application
This project entails the development of a sophisticated weather forecasting application utilizing data from a college’s weather station. The primary objective is to create a highly accurate machine learning model to predict temperature, wind speed and humidity. Leveraging Flutter for the frontend and TFLite for the backend, the application is designed to offer users a seamless and intuitive interface for accessing precise and reliable weather forecasts.

## System Architecture
The architecture is divided into the following modules as shown in Fig 4.1 :
 1. Data Collection Module: Collects real-time weather data from the college’s weather
 station.
 2. Data Processing Module: Preprocesses the raw data for further analysis.
 3. Machine Learning Module: Implements the time series forecasting model using con
volutional and LSTM layers.
 4. Mobile Application Module: Provides a user interface through Flutter.
 5. Integration Module: Uses TFLite to integrate the machine learning model with the
 mobile app.
![Screenshot 2024-06-07 225928](https://github.com/Rakshita2003/Weather-Forecasting-Application/assets/101338848/c9727a66-ed80-4874-a101-dc054f2df33f)

 ## Design Details
  Data Collection Module: The data collection module gathers weather data, including
 temperature, humidity, and wind speed, from the weather station and stores it in a
 structured format.
 
 Data Processing Module: This module handles data cleaning and transformation.
 Techniques such as normalization and missing value imputation are applied to ensure
 data quality.
 
 Machine Learning Module: The machine learning module uses a combination of
 convolutional layers and LSTM layers to build the forecasting model. The architecture
 is as follows:- Two convolutional layers with kernel size 2x2.
 18
- A max-pooling layer with pool size 2x2.- Flattening the data and repeating the vectors 30 times.
- Three LSTM layers with tanh activation functions and a dropout layer.
- A bidirectional LSTM layer with ReLU activation function.
- A dense (ANN) layer with ReLU activation function followed by an output node.
  
 The model is compiled using the ADAM optimizer and trained over 300 epochs.
 
 Mobile Application Module: The mobile application is developed using Flutter,
 providing an intuitive interface for users to interact with the weather forecasts. Key
 features include real-time updates, interactive visualizations, and customizable settings
 for weather alerts.
 
 Integration Module: TFLite is used to deploy the trained machine learning model
 within the mobile application. The .tflite model file is loaded into the Flutter project,
 and inference is run using the Tflite.runModel() method.

##  Integration with flutter UI using TFLite
This involves setting up a communication channel between the Flutter mobile applica
tion and the machine learning model running on a server. TensorFlow Lite (TFLite) is a powerful way to add AI capabilities to your mobile
 applications. TensorFlow Lite allows you to deploy machine learning models on mobile
 and embedded devices with low latency.

![Screenshot 2024-05-26 202355](https://github.com/Rakshita2003/Weather-Forecasting-Application/assets/101338848/cbacaafd-6a45-4e9f-abe3-8c97032b195b)

## Result

