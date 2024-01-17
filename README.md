# Stock Market Prediction Project

## Overview
This project focuses on predicting stock market prices, specifically for Bitcoin (BTC-USD), using a deep learning model implemented in Python with TensorFlow and Keras. The model employed for prediction is a Bidirectional LSTM (Long Short-Term Memory) neural network.

## Project Structure
The project consists of the following key components:

1. **Data Collection:** The historical stock market data for Bitcoin is loaded from the "stock-prediction_BTC-USD.csv" file.

2. **Data Preprocessing:** The data is preprocessed to scale the closing prices using Min-Max scaling. Sequences of data are created to train the deep learning model.

3. **Model Architecture:** The implemented neural network model utilizes Bidirectional LSTM layers with dropout for training. The architecture is as follows:
   - Input Layer: Bidirectional LSTM with return sequences
   - Hidden Layer: Bidirectional LSTM with return sequences and dropout
   - Hidden Layer: Bidirectional LSTM
   - Output Layer: Dense layer with linear activation

4. **Training:** The model is trained using historical data with a specified sequence length. The loss is calculated using mean squared error, and the Adam optimizer is employed.

5. **Evaluation:** The trained model is evaluated on the test set, and the performance is visualized by comparing actual and predicted prices.

## Dependencies
Ensure you have the following dependencies installed:

- TensorFlow (GPU version or CPU version)
- NumPy
- Pandas
- Seaborn
- Matplotlib
- Scikit-learn

You can install the necessary dependencies using the following:

```bash
pip install tensorflow
pip install numpy pandas seaborn matplotlib scikit-learn
```

## How to Run
1. Open the Jupyter notebook containing the provided code.
2. Run the notebook cell by cell, ensuring that there are no errors during execution.
3. Adjust parameters and experiment with the model architecture as needed.

## Results
The training history, loss curves, and a comparison of actual vs. predicted prices are visualized to assess the performance of the model.

## Author
Ved Prakash

Email- Vedprakash108.hitcse2020@gmail.com

Feel free to reach out with any questions or feedback!

*Note: Ensure that you have the necessary hardware requirements for running the code, especially if using the GPU version of TensorFlow.*
