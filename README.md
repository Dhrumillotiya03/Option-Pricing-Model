# Option-Pricing-Model
This repository shows Python implementations of the Monte Carlo simulation technique for option pricing, alongside the Black-Scholes pricing model. It features various examples and visualizations to illustrate how different option parameters affect simulated stock price trajectories. Additionally, the project incorporates the Black-Scholes formula to compute the theoretical values of European-style call and put options.

# Introduction
Monte Carlo simulation is a widely used numerical approach for estimating the value of financial derivatives, particularly options. It works by simulating numerous potential price paths for the underlying asset and computing the average expected payoff from these paths. The Black-Scholes model guides the stochastic behavior of the asset price, while the Monte Carlo method serves to approximate the option's fair value.

This method incorporates key variables such as the risk-free rate, current asset price, strike price, time to maturity, and the asset's return volatility to determine the option’s theoretical valuation.

# Implementation
The Jupyter Notebook Monte_Carlo.ipynb presents a Monte Carlo simulation for pricing European call options based on the Black-Scholes framework.

## Notebook Structure:
1) Library Imports: Essential Python libraries are loaded for numerical computation, random sampling, and data visualization.

2) Random Seed Initialization: A fixed seed is set to ensure that simulation results are reproducible.

3) Option Setup: Parameters such as the initial stock price (S0), strike price (K), time to maturity (T), risk-free interest rate (r), and volatility (sigma) are defined for use in option pricing.

4) Time Discretization: The number of time intervals (M) and corresponding time step size (dt) are specified to discretize the simulation horizon.

5) Simulating Asset Paths: Using the Black-Scholes model and its logarithmic form, asset price trajectories are simulated with efficient NumPy-based vectorized computations.

6) Estimating Option Value: The simulation computes the European call price by averaging the discounted payoff (max of final asset price minus strike) across all generated paths.

7) Displaying Results: The estimated call option price and the total computation time are output. Additionally, the notebook plots the first 10 simulated stock price paths.

8) Extended Scenarios: The notebook includes several variations where key option parameters (like volatility, strike, or maturity) are modified. For each scenario, the resulting option prices and sample path plots are generated to illustrate the sensitivity of the pricing to these inputs.

The notebooks demonstrate both the Monte Carlo simulation and the Black-Scholes pricing for a baseline set of option parameters. They display the estimated price of a European call option along with a graph of the simulated stock price trajectories. Subsequently, the notebooks run additional scenarios by adjusting key parameters to show how these changes influence the option's value, accompanied by updated plots of the corresponding stock price paths.

# Conclusion
This repository showcases how the Monte Carlo simulation and the Black-Scholes model can be applied to option pricing. It features Python code along with illustrative examples and graphs that help visualize the impact of varying option parameters on both the option value and asset price paths. By simulating numerous scenarios, the Monte Carlo approach offers a versatile and robust framework for valuing financial derivatives, making it highly valuable in risk assessment and pricing strategies within the finance sector.

