# Model of StockPred

This repository contains the saved models and necessary files for a stock prediction application. The application utilizes machine learning techniques to forecast stock prices based on historical data.

## Files Included
- **model**: This file represents the main model used for predictions. It contains the architecture and weights of the trained model.
- **best_model_v3.keras**: This file contains the best-performing model saved in Keras format. It can be loaded directly for further training or inference.
- **skala_X.json**: The skala_X.json file contains scaling parameters used to transform the input features (X) before they are fed into the model. This process typically involves normalization or standardization of the data, which aims to ensure that all features are on the same scale. This is important because machine learning models often perform better when the features are within a similar range.
- **skala_X.pkl**: A serialized version of the scaling parameters for easy loading and application during inference.
- **skala_Y.json**: The skala_Y.json file contains scaling parameters used to transform the target variable (Y) to a scale compatible with the model. This is especially important in regression cases, where the model's predictions need to be converted back to the original scale for accurate interpretation.
- **skala_Y.pkl**: A serialized version of the target variable scaling parameters, facilitating the inverse transformation of predictions.
- **tfjs_model**: This folder contains the model files converted for use with TensorFlow.js, allowing for deployment in web applications.
- **Training Results of Combined Model**: Shows images of the results of training

## Usage
- **Loading the Model**: Use the appropriate library (TensorFlow, Keras, etc.) to load the model files for predictions.
- **Data Preprocessing**: Ensure that the input data is preprocessed using the scaling parameters provided in Skala_X and Skala_X.pkl.
- **Making Predictions**: After loading the model and preprocessing the data, you can make predictions on stock prices.
- **Inverse Scaling**: Use skala_y and skala_Y.pkl to transform the predicted values back to their original scale for interpretation.

## Installation
To run this application, ensure you have the following libraries installed:
- **TensorFlow**
- **Keras**
- **NumPy**
- **Pandas**

You can install the required libraries using pip:
```sh
   pip install tensorflow keras numpy pandas
   ```


