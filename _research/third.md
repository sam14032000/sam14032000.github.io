---
title: "Stock market volatility prediction using VAR-ML hybrid model"
excerpt: "Volatility modelling has been an important part of financial modelling for a significant amount of time. Over the years GRACH model has been the go-to model for most analysts, since its explainable and robust. However, with the advent of machine learning, the accuracy of financial models has improved significantly. GARCH model usus the residual data from VAR or VECM models to capture information aboutunexpected shocks in the market. The aim of this study is to study the next-day prediction accuracy of RNNs, when the input data is the market volatiliity, as compared to, when VAR residual data is used additionally with market volatility. <br>
*Status: First draft completed. Under review by a journal.*<br/><img src='/images/data_pre.png'>"
collection: research
---

The study uses basic LSTM, GRU LSTM and bi-drectional LSTM models to compare the predictions made by two different data sets (Training period: 2008-2019; Test period: 2019-2020).
* The first dataset:
  * Input data: Indian stock market volatility; US, UK, Japan, China, Singapore, Hong Kong daily market data
  * Target Variable: Next day volatility of Indian stock market
* The second dataset:
  * Input data: VAR residuals for VAR fitted on India and each of the other six countries individually; Indian stock market volatility; US, UK, Japan, China, Singapore, Hong Kong daily market data
  * Target Variable: Next day volatility of Indian stock market

VAR residuals contain information about the response of a variable to a unexpected shock in the other variable. The other six countries were chosen as contributing variables since the nations are mostly developed or have a high volume of trade with India.

The hybrid model showed improved accuracy and increased senstivity to market shocks, proving the effectiveness of the hybrid model and the usefulness of residual data in volatility prediction.

### Best Performance: Bi-directional LSTM with the second dataset (Hybrid Model): RMSE = 0.00018
![Best Performance: Bi-directional LSTM with the second dataset (Hybrid Model)](/images/bilstm.png)

### Code Repository: [Click Here](https://github.com/sam14032000/volatility_prediction_study)
