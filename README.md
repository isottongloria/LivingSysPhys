# LivingSysPhys
In this repository, you will find the completed weekly exercises for the course on physical models of living systems taught by Professor Samir Suweis during the academic year 2023-2024 in Padova.

# Assignments

Homework 1 

1) Perform linear stability analysis of the deterministic logistic equation.

2) Perform the quasi stationary approximation of the consumer resource model with 1 species and 1 resources for the abiotic case. Check the analytical result with simulations.

3) Simulate the stochastic logistic model in your computer and check that the stationary distribution is a Gamma (in the case of linear (environmental) multiplicative noise) or P( n ) given by Eq. 2.25 in the notes for the sub-linear (demographic) multiplicative noise.

Homework 2

Plot both SAR and EAR as a function of the relative area, using the Log Series as the SAD distribution P( n ) = c (1-m)^n / n (c is the normalization constant - see Eq. 3.29). and compare it with a Power Law SAR of exponent z=0.25 (S(a)=k A^z) and k tuned so the be as close as possible to the solution for the random placement case. 

Homework 3

1) Choose a given type of ecological structure (e.g. mutualistic, or predator-prey, or etc...). Generate random matrices with for completely random and for the chosen ecological structures. You need to create SxS matrices (S is the number of species) with C non-zero entries and 1-C zeros (C is the connectivity between 0 and 1). The non-zero elements are drawn at random from given distributions. Depending on the network structure some symmetries and constraints may hold. fix C and for S=20, 50, 100, 200 calculate the eigenvalues of the matrix and plot them against Real part (x-axis) and imaginary part (y-axis).

2) plot the maximum real part eigenvalues for each S (Max Re lambda as a function of S) and the probability of P(lambda >0) as a function of the proper control parameter (e.g. for the complete random case is sigma*(S*C)^0.5. Compare these plots with the one for the complete random case (the original May case).

3) Optional: how the eigenvalues of the Jacobian of a GLV with constant growth rate set to 1 and random positive x^* (for example taken from a Uniform distribution between 1 and 10) and random interactions are distributed? Does the circular or elliptic law still hold? And what about the stability-complexity paradox?

Homework 4

Using non-homogeneous Poisson process, generate the spike train of 100 neurons (if your code is efficient you can also do more, e.g. 200 or 1000sorridente

Do this for two different situations:

1) The firing rate $\lambda_t$ is independent for each neuron, and generated as random variables extracted each time step by an exponential distribution $p(\lambda_t) r exp [- r \lambda_t]$ with r=0.1. 

2) The firing rate $\lambda_t$ is the same for each neuron, and generated as random variables extracted each time step by an exponential distribution $p(\lambda_t) r exp [- r \lambda_t]$ with r=0.1. 

For both cases you can use a time step dt=0.01. I remember you that the probability of a spike is $\lambda_t * dt$. Do at least 1000 timesteps.

What is the differences in terms of neural avalanches for the two cases? You can, if you want, characterize the avalanches size distributions, remembering that an avalanche size is defined the total number of neurons spiking between to period of total silence (no neurons spiking).

Optional: compute the avalanche durations analytically using the same parameters of the simulations for the two cases. The full calculations are available in the notes.

Homework 5

 Perform the stability analysis for the Wilson-Cowan model without refractory dynamics.  Set self-excitation and self inhibition to zero, and the alpha_E=alpha_I=1.
Optional: what is the difference if one considers also the refractory dynamics?

Homework 6

 Play with the Hopfield network code and/or the Jansen and Rit model code. Understand the code, and play with it. Generate some output (e.g. retrieve the memory input from the Hopfield network).

As an output, you can simply send me a doc/pdf file writing a couple of paragraph, explaining me what you have done, and what you have learn. It is enough half a page.

Homework 7

Choose one of the examples on feedback loop (can be either negative positive) and simulate it. Try to combine two feedback loop (or simulating the genetic network shown in class or creating one yourself), simulate it and describe in few sentences the results of the simulations.

