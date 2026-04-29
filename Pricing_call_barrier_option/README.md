## Project Overview

In this project, we simulate a Lévy process and use it to price an up-and-out barrier call option. We first show that generating the process through exponential waiting times is equivalent to using a uniform distribution for jump occurrences. Based on this, we proceed with the simulation using the parameters defined below.

We consider the time interval \( I = [0,1] \) and simulate the price process of the up-and-out call option using an exponential Lévy process on this interval.

## Model Parameters

- Drift: \( b = 0.05 \)  
- Volatility: \( \sigma = 0.2 \)  
- Jump intensity: \( \lambda = 5 \)  
- Jump size distribution: \( Y_i \sim \text{Laplace}(0, 0.1) \)  
- Initial price: \( S_0 = 100 \)  
- Strike price: \( K = 50 \)  
- Barrier level: \( H = 80 \)  
- Number of Monte Carlo paths: 500  
- Interest rate: \( r = 5\% \)

## Result

The estimated price of the up-and-out call option is:

**\( C = 58.23 \)**