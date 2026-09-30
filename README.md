# Forecasting UK refugee numbers: ARIMA, SVM and LSTM

Annual refugee numbers in the United Kingdom from 1950 to 2016, forecast with three model families and compared on a held-out test split (last 20% of the years). Written in R.

- ARIMA: ARIMA(0,0,4) and ARIMA(2,2,0) with residual diagnostics. ARIMA(0,0,4) is the better of the two (test RMSE 117,936 against 535,303).
- SVM: grid search over kernel, cost and gamma. Fits the training data well but does not generalise to the test years.
- LSTM: a small stateful Keras network. Test RMSE 13,360, by far the best of the three, and its forecast follows the actual trend and fluctuations closely.

Also on [Kaggle](https://www.kaggle.com/code/tarktunataalt/forecasting-uk-refugee-numbers-arima-svm-lstm).
