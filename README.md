# Black-Scholes-Model-implementation
 the project contains 2 implementation 1 being the implementation on sample values irrespective of intrerest rares, dividends, ETC parameters 
 2nd being the commplete implementation with the externnal parameters like intrerest rares, dividends, ETC 

Black scholes merton model:-
The Black-Scholes-Merton model is a mathematical formula used to calculate the theoretical price of options contracts. It also provides option Greeks, which are measures of the sensitivity of an option's price to changes in various factors. Here's an overview of the model, its formula, and how to implement it in Python:

Black-Scholes-Merton Formula:
For a European-style call option:
C = S * N(d1) - X * e^(-r * T) * N(d2)

For a European-style put option:
P = X * e^(-r * T) * N(-d2) - S * N(-d1)

Where:
C = Call option price
P = Put option price
S = Current price of the underlying asset
X = Strike price of the option
r = Risk-free interest rate
T = Time to expiration in years
N(d) = Cumulative standard normal distribution function
d1 = (ln(S / X) + (r + (σ^2)/2) * T) / (σ * sqrt(T))
d2 = d1 - σ * sqrt(T)

Option Greeks:
Delta (Δ): Measures the change in the option price for a one-unit change in the price of the underlying asset.
Gamma (Γ): Measures the change in the option's delta for a one-unit change in the price of the underlying asset.
Vega (ν): Measures the change in the option price for a one-percentage-point change in implied volatility.
Theta (θ): Measures the change in the option price over time as the time to expiration approaches.
Rho (ρ): Measures the change in the option price for a one-percentage-point change in the risk-free interest rate.
