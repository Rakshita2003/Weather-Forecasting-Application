# Weather-Forecasting-Application
This project entails the development of a sophisticated weather forecasting application utilizing data from a college’s weather station. The primary objective is to create a highly accurate machine learning model to predict temperature, wind speed and humidity. Leveraging Flutter for the frontend and TFLite for the backend, the application is designed to offer users a seamless and intuitive interface for accessing precise and reliable weather forecasts.

## Project Highlights
- Real-time data collection (temperature, humidity, wind speed).
- Data cleaning and preprocessing (normalization, missing value imputation).
- Utilized a hybrid model combining Convolutional and LSTM layers.
- Trained the model for 300 epochs using the ADAM optimizer.
- Deployed ML model using TensorFlow Lite.
- Developed with Flutter having key features: Real-time updates, interactive visualizations, customizable alerts and Dark-Light Modes for better user experience.
- Integrated with wiredash.com for feedback and email notifications.

## System Architecture

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
### Temperature:
![Screenshot 2024-04-19 003856](https://github.com/Rakshita2003/Weather-Forecasting-Application/assets/101338848/7990bd34-a3ef-4741-b35f-34798ad0fba2)

### Humidity:
![Screenshot 2024-04-19 003836](https://github.com/Rakshita2003/Weather-Forecasting-Application/assets/101338848/67600b03-bfa7-4e8f-bbca-aa1a5344e656)

### Wind Speed:
![Screenshot 2024-04-19 003816](https://github.com/Rakshita2003/Weather-Forecasting-Application/assets/101338848/791d5805-09c9-4a62-936d-0bdaa9be9f97)

## App UI :

![Screenshot 2024-05-23 123826](https://github.com/Rakshita2003/Weather-Forecasting-Application/assets/101338848/27c57cf3-1de2-4226-b19e-86b5062d03fc)
![Screenshot 2024-05-23 124452](https://github.com/Rakshita2003/Weather-Forecasting-Application/assets/101338848/6d4c415b-1355-4790-802c-eb8c484b1a4e)
![Screenshot 2024-05-23 130142](https://github.com/Rakshita2003/Weather-Forecasting-Application/assets/101338848/2a1e56f4-6e72-4bcc-8338-92ef86eb667f)
![Screenshot 2024-05-23 132159](https://github.com/Rakshita2003/Weather-Forecasting-Application/assets/101338848/7e9b95f6-1d6b-4dea-a549-9f4c7e21ee9a)

So, this app has Dark and Light Mode enabled for better user experience, catering to
 different preferences and environments. The Dark Mode provides a visually comfortable
 experience in low-light conditions, reducing eye strain and improving readability, while
 the Light Mode offers a traditional bright interface suitable for well-lit environments.
 Aditionally, we’ve crafted an intuitive feedback page tailored to seamlessly integrate
 with wiredash.com, serving as our database solution. This strategic implementation en
sures that every user interaction is meticulously captured, enabling swift communication
 through email notifications as users submit their feedback.
