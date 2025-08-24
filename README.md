# Predicting-Orange-Stock-Price-Using-an-LSTM-Deep-Learning-Model
Orange Stock Price Prediction Using an LSTM Deep Learning Model
This project showcases my ability to apply deep learning techniques to a classic problem in financial markets: stock price prediction. Using a Long Short-Term Memory (LSTM) neural network, a type of model specifically designed for sequential data, I developed a robust forecasting solution for the stock price of Orange S.A. (ORA.PA). This project is a demonstration of my skills in data science, time series analysis, and practical machine learning model development.

Project Overview
The goal was to build a model that could learn from historical stock price trends and forecast future movements. My approach followed a standard but rigorous machine learning pipeline:

Data Acquisition & Preparation: I used the yfinance library to fetch a comprehensive history of Orange S.A. stock data. To prepare the data for the LSTM model, I isolated the Close price and normalized it using a MinMaxScaler. This crucial step ensured that the model's training process was both stable and efficient.

Feature Engineering: A core step in time-series forecasting is structuring the data. I created a "lookback window" of 60 days, transforming the data into sequences where the model learns to predict the price on day t+1 based on the prices from days t-59 to t.

Model Architecture: The predictive power comes from a stacked LSTM network built with TensorFlow/Keras. My architecture consists of three LSTM layers followed by a Dense output layer. To prevent overfitting and ensure the model generalizes well to unseen data, I strategically incorporated Dropout layers.

Training & Validation: The model was trained with the Adam optimizer and Mean Squared Error (MSE) loss. I employed an EarlyStopping callback to monitor the validation loss, a key technique to automatically stop training once the model's performance on new data ceases to improve.

Results: The model successfully learned the underlying patterns in the stock data. Its performance was quantified by a final Root Mean Squared Error (RMSE) of approximately 0.26, indicating a strong predictive capability. The visualization of predicted vs. actual prices confirms the model's ability to track and forecast price movements accurately.

Key Takeaways & Skills Demonstrated
Time-Series Analysis: I gained hands-on experience in preparing and modeling time-series data, a fundamental skill in many data science domains.

Deep Learning Expertise: This project showcases my proficiency in designing, implementing, and training a complex deep learning model using TensorFlow/Keras.

Practical Problem-Solving: From data acquisition to model evaluation, I demonstrated the ability to tackle a real-world problem from end to end, making logical decisions at each stage of the process.

Code Quality: The project is well-documented and structured, reflecting my commitment to clean and reproducible code.

This LSTM model serves as a robust foundation, and it can be further improved by incorporating additional features like technical indicators or sentiment analysis. It represents a solid step in my journey toward building more advanced predictive systems.
