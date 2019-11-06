# Statistics-for-Data-Science
CS 6313 - The University of Texas at Dallas 

## Mini project 1
1. (10 points) Consider Exercise 4.11 from the textbook. In this exercise, let XA be the
lifetime of block A, XB be the lifetime of block B, and T be the lifetime of the satellite.
The lifetimes are in years. It is given that XA and XB follow independent exponential
distributions with mean 10 years. One can follow the solution of Exercise 4.6 to show
that the probability density function of T is
fT (t) = (
0.2 exp(−0.1t) − 0.2 exp(−0.2t), 0 ≤ t < ∞,
0, otherwise,
and E(T) = 15 years.

(a) Use the above density function to analytically compute the probability that the
lifetime of the satellite exceeds 15 years.
(b) Use the following steps to take a Monte Carlo approach to compute E(T) and
P(T > 15).
i. Simulate one draw of the block lifetimes XA and XB. Use these draws to
simulate one draw of the satellite lifetime T.

ii. Repeat the previous step 10,000 times. This will give you 10,000 draws
from the distribution of T. Try to avoid ‘for’ loop. Use ‘replicate’ function
instead. Save these draws for reuse in later steps. [Bonus: 1 bonus point
for not taking more than 1 line of code for steps (i) and (ii).]

iii. Make a histogram of the draws of T using ‘hist’ function. Superimpose the
density function given above. Try using ‘curve’ function for drawing the
density. Note what you see.

iv. Use the saved draws to estimate E(T). Compare your answer with the exact
answer given above.

v. Use the saved draws to estimate the probability that the satellite lasts more
than 15 years. Compare with the exact answer computed in part (a).

vi. Repeat the above process of obtaining an estimate of E(T) and an estimate
of the probability four more times. Note what you see.

(c) Repeat part (vi) five times using 1,000 and 100,000 Monte Carlo replications
instead of 10,000. Make a table of results. Comment on what you see and
provide an explanation


2. (10 points) Use a Monte Carlo approach estimate the value of π based on 10, 000
replications. [Ignorable hint: First, get a relation between π and the probability
that a randomly selected point in a unit square with coordinates — (0, 0), (0, 1),
(1, 0), and (1, 1) — falls in a circle with center (0.5, 0.5) inscribed in the square.
Then, estimate this probability, and go from there.]

## Mini project 2
1. (12 points) Consider the dataset roadrace.csv posted on eLearning. It contains
observations on 5875 runners who finished the 2010 Beach to Beacon 10K Road Race
in Cape Elizabeth, Maine. You can read the dataset in R using read.csv function.
(a) Create a bar graph of the variable Maine, which identifies whether a runner is
from Maine or from somewhere else (stated using Maine and Away). You can
use barplot function for this. What can we conclude from the plot? Back up
your conclusions with relevant summary statistics.

(b) Create two histograms the runners’ times (given in minutes) — one for the
Maine group and the second for the Away group. Make sure that the histograms
on the same scale. What can we conclude about the two distributions? Back
up your conclusions with relevant summary statistics, including mean, standard
deviation, range, median, and interquartile range.

(c) Repeat (b) but with side-by-side boxplots.
(d) Create side-by-side boxplots for the runners’ ages (given in years) for male and
female runners. What can we conclude about the two distributions? Back up
your conclusions with relevant summary statistics, including mean, standard
deviation, range, median, and interquartile range.


2. (8 points) Consider the dataset motorcycle.csv posted on eLearning. It contains
the number of fatal motorcycle accidents that occurred in each county of South Carolina during 2009. Create a boxplot of data and provide relevant summary statistics.
Discuss the features of the data distribution. Identify which counties may be considered outliers. Why might these counties have the highest numbers of motorcycle
fatalities in South Carolina?

## Mini project 3 
1. (8 points) Suppose we would like to estimate the parameter θ (> 0) of a Uniform (0, θ) population based on a random sample X1, . . . , Xn from the population. In the
class, we have discussed two estimators for θ — the maximum likelihood estimator,
ˆθ1 = X(n), where X(n) is the maximum of the sample, and the method of moments
estimator, ˆθ2 = 2X, where X is the sample mean. The goal of this exercise is to
compare the mean squared errors of the two estimators to determine which estimator
is better. Recall that the mean squared error of an estimator ˆθ of a parameter θ is
defined as E{(ˆθ − θ)^2}. For the comparison, we will focus on n = 1, 2, 3, 5, 10, 30 and θ = 1, 5, 50, 100.

(a) Explain how you will compute the mean squared error of an estimator using
Monte Carlo simulation.

(b) For a given combination of (n, θ), compute the mean squared errors of both ˆθ1
and ˆθ2 using Monte Carlo simulation with N = 1000 replications. Be sure to
compute both estimates from the same data.

(c) Repeat (b) for the remaining combinations of (n, θ). Summarize your results
graphically.

(d) Based on (c), which estimator is better? Does the answer depend on n or θ?
Explain. Provide justification for all your conclusions.


2. (12 points) Suppose the lifetime, in years, of an electronic component can be modeled by a continuous random variable with probability density function
f(x) = (
θ
xθ+1 x ≥ 1,
0, x < 1,

where θ > 0 is an unknown parameter. Let X1, . . . , Xn be a random sample of size
n from this population.
(a) Derive an expression for maximum likelihood estimator of θ.

(b) Suppose n = 5 and the sample values are x1 = 21.72, x2 = 14.65, x3 = 50.42, x4 =
28.78, x5 = 11.23. Use the expression in (a) to provide the maximum likelihood
estimate for θ based on these data.

(c) Even though we know the maximum likelihood estimate from (b), use the data in
(b) to obtain the estimate by numerically maximizing the log-likelihood function
using optim function in R. Do your answers match?

(d) Use the output of numerical maximization in (c) to provide an approximate
standard error of the maximum likelihood estimate and an approximate 95%
confidence interval for θ. Are these approximations going to be good? Justify
your answer.

## Mini project 4


## Mini project 5


## Mini project 6 
