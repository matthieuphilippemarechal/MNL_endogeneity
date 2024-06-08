We consider a Multinomial Logit with the following utility functions:

U_walk = beta0_walk + beta1 * X_walk + beta2 * C_walk + eps_walk
U_metro = beta0_metro + beta1 * X_metro + beta2 * C_metro + eps_metro
U_car = beta0_car + beta1 * X_car + beta2 * C_car + eps_car

X_m is the time for travelling using mode m and C_m is the cost for travelling using mode m. 

In our simmulation, true parameters are: beta0_metro = 0.7, beta0_caminata = 0.4, beta0_auto = 0,beta1 = -0.02 (sensitivity to time travel),
beta2 = -0.04 (Sensitivity to cost travel). 

The variable X_car is assumed to be endogenous, with the instrumental variable D_car representing distance. The relationship between D_car and X_car is given by: 
X_car = a_auto * D_auto + v_auto + eta_auto where a_auto = 1/25, v_auto and eta_auto are normally distributed with mean values of zero. We assume that eps_walk, 
eps_metro and eps_car + beta1 * eta_auto follow Gumbel distributions with the same variance.

We estimate the parameters beta0_walk, beta0_metro, beta0_car, beta1 and beta2 using four estimators: Maximum Likelihood, Control Function, Method of Moments, 
and Two-Step Estimation. The latter two methods exhibit the smallest bias.
