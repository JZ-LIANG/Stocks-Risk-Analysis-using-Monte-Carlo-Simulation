# Stocks Risk Analysis using Monte Carlo Simulation

In this notebook, we focus on using Monte Carlo Simulation and Multiple Linear Regression to analysis financial risk on stocks portfolio.


<figure>
  <img src="images/simulate_img.png" width="800" alt="Simulate the Market Factors" title="Simulate the Market Factors" />

</figure>
<p align="center"> Simulate the Market Factors </p>

<br><br>
The goal of this demo is to build a predicion model able to indicate the **VaR (Value at Risk)** for a given stock portfolio: in other words, an indicator of how much the global value of our stocks will increase/decrease in a given time interval. To be more precise, the VaR indicates (with a given confidence level) the expected lower bound of the losses we can expect.


Notebook can be divided into three parts:

 * First we define relationship between market factors and instrument's returns. We choose to use Ordinary Least Square (OLS) regression model to estimate the weights for each instrument as a linear function of market factors.

 * Defining the distributions for the market factors. Since the distributons of those factors are unknow, we can only approximate their distribution. Weuse the Kernel density estimation (KDE) technique to approximate such distributions.

* After we got "elationship between market factors and instruments" and "distributions for the market factors", we could Generate samples of instrument value by running a huge number of simulations, and finally calculate the Var.




