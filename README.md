# Stock Price Prediction using LSTM
#![image](https://github.com/charliethomasct82/Research_Thesis/assets/93368865/0ff1f29c-11a3-4349-bc54-8d6400e99b53)


Stock price prediction has welcomed the development of advanced capabilities due to the speedy development of machine learning techniques and Artificial Intelligence, Improved computational speed, and ever-increasing data Availability. The stock market has become more volatile and complex due to access to investment opportunities is easier in current times. This research compares three different types of LSTM architecture(single-layer, multi-layer, and bi-directional) to predict the stock price of Indian banking stock, Yes Bank Ltd. The Structure of the Thesis is as follows: Chapter is 1, an introduction to the Thesis carried out; Chapter 2 , highlights the review of the Literature in the studied area; Chapter 3, explores the Research Methodology; Section 4, describes the Analysis of the study; Section 5, Results of the analysis are discussed; conclusions and future work are presented in Chapter 6, followed by references, and appendices.

The study uses predictors such as Historical prices(open, close, high, and low). Historical price information has been extracted from the Yahoo finance data by using the yfinance library for the period from 2005-05-07 to 2023-08-09. The bi-variate analysis highlights the high correlation between historical price features. Hence Date and Close price were utilized for further analysis. Data was transformed using a combination of Log-square root transformers to make the data stationary. A new Data set with features Date, input_1, Input_2, Input_3 and Target was created by the feature engineering process. Three baseline models and 45 experimental models with different combinations of batch size and number of epochs were built and compared on the performance based on MSE(Loss on validation data). A bidirectional LSTM with 10 epochs and 64 batch size was selected for hyperparameter tuning because of the low score of MSE(validation data). The hyperparameter tuning will be performed to get the most optimized model to predict the stock price. Hyperparameter tuning has improved the Loss by 88.28% from 322.02 to 37.88 (refer to Plot 4.9.1). A tuned Bi-directional model was proposed to be implemented on unseen/ test data. The proposed model was able to predict the price with a loss of 25.024 and within the average value of 5.002(refer to Plot 4.10.1)(refer to table 5.3.1). The Proposed model was also able to predict the trend closely to the real trend(refer to plot 5.3.1). This paper established that simple LSTM architecture such as single-layer LSTM was less efficient than complex LSTM architecture such as multi-layer LSTM and bi-directional LSTM. This study also established that bi-directional LSTM was able to predict the trend of the moment of the stock efficiently(refer to plot 5.3.1).
