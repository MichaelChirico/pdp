[![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/pdp)](https://cran.r-project.org/package=pdp)
[![Build Status](https://travis-ci.org/bgreenwell/pdp.svg?branch=master)](https://travis-ci.org/bgreenwell/pdp)
[![Coverage Status](https://img.shields.io/codecov/c/github/bgreenwell/pdp.svg)](https://codecov.io/github/bgreenwell/pdp?branch=master)
[![Downloads](http://cranlogs.r-pkg.org/badges/pdp)](http://cranlogs.r-pkg.org/badges/pdp)
[![Total Downloads](http://cranlogs.r-pkg.org/badges/grand-total/pdp)](http://cranlogs.r-pkg.org/badges/grand-total/pdp)
[![Rdoc](http://www.rdocumentation.org/badges/version/pdp)](http://www.rdocumentation.org/packages/pdp)

# pdp: An R Package for Constructing Partial Dependence Plots

Complex nonparametric models---like neural networks, random forests, and support vector machines---are more common than ever in predictive analytics, especially when dealing with large observational databases that don't adhere to the strict assumptions imposed by traditional statistical techniques (e.g., multiple linear regression which assumes linearity, homoscedasticity, and normality). Unfortunately, it can be challenging to understand the results of such models and explain them to management. Partial dependence plots offer a simple solution. Partial dependence plots are low-dimensional graphical renderings of the prediction function $\widehat{f}\left(\boldsymbol{x}\right)$ so that the relationship between the outcome and predictors of interest can be more easily understood. These plots are especially useful in explaining the output from black box models. The `pdp` package offers a general framework for constructing partial dependence plots for various types of fitted models in R. 

A detailed introduction to `pdp` has been accepted for publication in The R Journal; a preprint is available [here](https://github.com/bgreenwell/pdp-paper/blob/master/RJwrapper.pdf). You can track development on  at https://github.com/bgreenwell/pdp. To report bugs or issues, contact the main author directly or submit them to https://github.com/bgreenwell/pdp/issues. 

As of right now, `pdp` exports four functions:

* `partial` - compute partial dependence functions (i.e., marginal effects) for various model fitting objects;
* `plotPartial"` - plot partial dependence functions (i.e., marginal effects) using `lattice` graphics;
* `autoplot` - plot partial dependence functions (i.e., marginal effects) using `ggplot2` graphics;
* `topPredictors` extract most "important" predictors from various types of fitted models.

## Installation

The `pdp` package is [currently listed on CRAN](https://CRAN.R-project.org/package=pdp) and can easily be installed:
```r
  # Install from CRAN (recommended)
  install.packages("pdp")
  
  # Alternatively, install the development version from GitHub
  devtools::install_github("bgreenwell/pdp")
```

