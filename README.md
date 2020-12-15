# Forecasting exchange rates and stock prices using stochastic processes
Nowadays, more and more people are investing in investments, which raises a problem: How to find interesting investment instruments and how to predict how they will behave in the future? To answer this question, we turn to the models from the course on random processes. To begin with, let's understand how the process describes the price of stocks, currencies. If the values ​​of a variable change unpredictably over time, then they say that it obeys a stochastic process.

We will predict the stock price using the Ito formula, which is widely used to model the stock price.
This formula is based on two important values. It is the volatility and profitability that needs to be found so that we can make calculations with our original formula. Volatility in a broad sense is a measure of the risk of an investment. The higher the volatility, the higher the risk, but also the higher the return. Indeed, the fundamentals of corporate finance are based on the fact that profitability grows with increasing risk. You can also understand volatility using the experiment of throwing a ball into holes. You can see this in detail with illustrations in the notebook file. All formulas, definitions are also described in detail in this file.
We calculate the profitability using the CAPM financial model.
Having calculated the profitability and volatility, we can insert them into our formula, and then we will already receive a ready-made formula for predicting the rate for a particular asset.

We also wrote a program that visualizes the trajectories of a random process and gives the final value of the stock rate.
But so that we can understand how well our model works, we wrote a program that makes predictions using machine learning. We have made a program that predicts the dollar rate, which strongly depends on the oil rate. We took the oil grade Brent. We used the yahoo finance database for prediction, but it is not complete enough to make a good prediction. Therefore, we decided to take data from specific databases that track the required values. It can be considered using the example of the forecast of the Russian RTS index

As a result, having tested our model on several assets, we got that it works quite accurately.
For example, the correlation of the dollar exchange rate forecast with true exchange rate values ​​was about 0.8, which is a good result and which confirmed our assumptions about the dependence of the Russian eeonomy on oil. True, our model works well in non-crisis times, perhaps it can give an accurate result in times of crisis, but still it works better in non-crisis times.

Thus, we have defined the rate prediction model. All theoretical and computational details can be found in the ipynb file.

If you have any questions, I am happy to answer them. Write to mail: osipyan.tr@phystech.edu
Thanks for attention!
