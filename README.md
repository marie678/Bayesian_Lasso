# Bayesian_Lasso
This is a project on the Bayesian Lasso for our class on Bayesian Statistics at ENSAE


The standard linear models tend to perform poorly when dealing with large datasets, notably with 
high-dimensional data where the number of variables exceeds the number of observations, as well
as in the presence of multicollinearity in the explanatory variables. Penalized regressions aim to
fix these issues by adding penalty terms on the complexity of linear regression models, to address
multicollinearity and overfitting (e.g., Ridge, Lasso). The penalty takes the form of a constraint in
the regression equation, which reduces (shrinks) the coefficients’ values towards zero, and therefore
penalizes the model for having too many variables. This is known as shrinkage or regularization.
A main issue of the frequentist Lasso raised by Kyung et al. (2010), is that it provides point
estimates for coefficients, but does not offer a statistically valid method to obtain standard errors for
these estimates, especially for coefficients shrunk to zero. As a result, Kyung et al. developed a
Bayesian Lasso, which treats the Lasso’s penalty term as a Laplace prior in a hierarchical model. This
approach provides valid uncertainty estimates (e.g. standard errors) for all coefficients, including
those shrunk to zero, thereby addressing a key limitation of the frequentist Lasso.
In this project, we implement both a Bayesian and a frequentist Lasso, and compare their estimations,
applied to several specific regression cases with simulated data.
