# More Math

## Taylor Series
For a function Real number, f in set C to infinity, the Taylor series f at x_0 is

T_infinity(x) = Sum(inf, k=0)...


## Differentiation Rules

- Review Partial Differentation 

# Probabilities

*Sample Space*: set of all possible outcomes of realizations
Example: Tosss a coin rwice, sample sapce is  Ome = {HH HT, TH, TT}

*Event*: A sbust of sample space
Example: the event at least one toss is a ead is A = {HH, HT, TH}

*Probabilit*: We assign a real number P(A) to each event A, called probability of A.

*Probability Axioms* The probability P must satisfy three axioms
- P(A) >= 0 for every A
- P(om) = 1
- If A2, A1,.... are disjointd, then P(U^inf_i=1 A_i) = Sum(inf, i=1, P(A))

## Ramdom Variable

*Definitions*: A random vairable is a measurable functionn that maps aa probability space into a medsurable space, i.e. X:Omega -> R, thaty ssigns real number X(omega) to each outcome omega.

Example: If OMEGA = {(x,y_: x^2 + y^2 <= 1} and our outcomes are samples (x,y) from unit disk, then these are some examples of random variables X(oomega) = x, y(omega) = , Z(omega) = x + y

*Data and Stats*: Te data are specific realizations of random vairable; A stats is just any function of the data or random variable

## Distribution Function*

*Definition*: Suppose X is a random variable, x is apscific value of it, Cumulative distribution function (CDF) is the function F: R -> [0, 1]. where F(x) = P(X <= x).

if X is discrete implises parobbility mass function: f(x) = P(X =x)

If X is continous -> Probability density function for X if there exists a function f such tat f(x) >= 0 for all x, der(inf, -inf, f(x)) and for every a <= b, P(a<= x<=b) = der (a, b, f(x))

if F(x) is differentialble everywhere

## Distribution Function
*Definition*: Suppose X is a radndom variable, x is a specific va;ie pf lor, weere F(x) -

## Common Distributions
- Uniform
- Binomial
- Geometric x ~ Poisson(lamda)
- Posson X ~ Ooisson(lamada)

### Continuous variable
- Uniform
- Gaussian
- Gamma
- Exponential

## Mutibartiate Distributioon 

## Correlation
- Covairance cov(X, Y) = E[(X - mul_x)(Y-mul y)]
- Correlation coefficent: corr(X, Y) = Cov(X, Y-|delta_x*Delta_y

Independence => Uncorrelated (coor(X, Y)=0)


## Exponential family
*Defintion* A faily of pdf or pmf s is called an exponential family if f(x/theta) = h(x)c(rt

## Optimization
*Def*: Optimization refer s to choosing the best element from some set available alternative. A general form is as follows.
*Covex Optimization*: Convex Fucntions: if for any two points x_a and x_2 in its domain X and any t in set [0. 1]
- A function f is said to be conczave if -f is convex
*Convex Set* a set S is convex if and only if for x_1, x_2 in set S,...
Convex Optimization: is minimization of a convwx function over a convex set
*Pupular convex optimization algos*
- Gradient descent
- Conjugate gradient
- Newton's method
- Quasi-Newton method
- Subgradent method


# DL
## Datasets
Trainning Data
- N samples/instances D^Train = {(x_1, y_1),(x_2, y_2), ..., 
- They are used for learning f(`)
Test data
- M samples/instances D^TEST = {(x_1, y_1),(x_2, y_2), ..., (x_m, y_m))
- They used for access how well f(`) will do.

## Development/Validation data
- L samples/instances: D^Dev = {(x1, y1), (x2, y2), ..., (x_L, y_L)}
- They are used to optimize hyper-parameter

If we don't have a development set
We use *S-fold Cross Validations*
- Split trainning data into S eaul parts
- Use each pary in turn as a dvelopment dataset and use the th;er as a train dataset
- Choose the hyper-parameter leading to best average performace.

Special case: S = N, called leave-one-out

## Expected Risk
For a loss function L(y', y)
- eg. L(y', y) = I[y' != y], called 0-1 loss
- many more other losses are qw qill aww
the expected risk of f is defined as
R(f) = E(x, y)~pL(f(x), y)
- expecatation of error is the expect risk 
- training error can sometimes be agood proxy of expected risk


## High level picture
Typical steps of developing a machine learning system:
- Collect data, split into training, development, and test sets
- Train a model with a machine learning algorithm. Most often we apply cross-validation to tune hyper-parameters
- Evaluate using the test data and report performance
- Use the model to predict future/make decisions


