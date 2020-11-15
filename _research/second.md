---
title: "Recession Prediction using Markov Regime Switching Model"
excerpt: "Based on the business cycle theory, every economic recession and expansion is just part of a cyclic process. Hence it is a fair to treat different parts of the cycle as seperate regimes, where the economy resides. Over the years bond yield has acted like a measure for market sentiment and an indicator for recessions.We test the capability of bond yields in predicting recessions in multiple countries, by using a modification of the model, which uses external regressors to calculate a [time varying transition probability](https://www.kansascityfed.org/publicat/reswkpap/pdf/rwp98-09.pdf) developed by Andrew J. Filardo. Below is the image of predictions made by the model for USA. <br>
*Status: First draft completed. Under review by supervising professor.*<br/><img src='/images/markov_switch.JPG'>"
collection: research
---

Over the years economies over the world have gone through several recessions. Every recession has had a different causal factor, something that triggered the event. In the 1930s depression, it was a combination of the Federal policies in US with the gold tariff laws, and in 2008, it was the failure of housing finance market due to mortgage debts that triggered the recession and sent the market into a free fall. Hoever, there was a commmon effect that is observed before the recessions, which is a downturn in investor sentiment. Before recessions, investors often change their habits and focus on more secure financial assets like bonds. Due to this change, variables associated with such assets also show different patrerns than ususal.

An example of such change is the rise in yield spreads. Whenever the bond yield curve inverts, it suggests a abnormal market position, and the yield spread rises. Every recession since the 1990s has witnessed an inversion of the curve before a recession, however a curve inversion is not a definite indicator. Inversion should occur for a certain time and upto a certain intensity for it to signal a recession. Capturing this signal, using yield spread as an exogenic regressor on GDP, is the aim of this study. The Markov Switching model with time varying transition probabilities ([Andrew J. Filardo, 1998](https://www.kansascityfed.org/publicat/reswkpap/pdf/rwp98-09.pdf)) is an appropriate model to do so. The model constructs the transition matrix for each point in time slice by assuming the switch variable to be a markov process. The switch variable signals a change in the regime. In Filardo's model, the switch variable is a markov process and can be influeneced by the external regressor, which can be an indicator of the status of nation's ecnonomy. In out case, the external regressor was the 10 year-3 month yield spread. 

We study the efficacy of yield spread as a recession indicator, by applying the model first on data from USA (baseline), since investors in developed markets are often more disciplined and focus on such indiactors. Following this, the model is applied on three developing countries, to test whether this simple model can be accurate in predicting recession time periods.

Results: **India**
![India](/images/ind5.png)
**South Africa**
![South Africa](/images/sa5.png)
**South Korea**
![South Korea](/images/sk5.png)
