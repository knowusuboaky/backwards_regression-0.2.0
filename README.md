# Backwards Regression Python Library Version 0.2.0 - Automated feature selection in linear and logistic regression models. 

The Backwards Regression Python Library is an open-source toolkit for automated feature selection in regression models. It supports both linear and logistic regression, dynamically selecting the appropriate method based on the target variable, and allows users to specify the optimization method.

## Installation
```bash
pip install backwards_regression==0.2.0
```

## Load Package
```bash
## Load Package
from backwards_regression import fit_logistic_regression
from backwards_regression import fit_linear_regression
```

## Usage
```bash
## (Linear) With interactions included - set to True and Without Interactions included - set to False
result, dropped_vars = fit_linear(X, y, threshold_in=0.01, threshold_out=0.05, include_interactions=True, verbose=True, method='pinv')

## Print Selected features
print("Final included features:", result)

## Print Eliminated features
print("Dropped variables:", dropped_vars)
```
```bash
## (Logistic) With interactions included - set to True and Without Interactions included - set to False
result, dropped_vars = fit_logistic(X, y, threshold_in=0.01, threshold_out=0.05, include_interactions=True, verbose=True, method='bfgs')

## Print Selected features
print("Final included features:", result)

## Print Eliminated features
print("Dropped variables:", dropped_vars)
```

## Key Features
- Automated backward regression for linear and logistic regression models.
- Inclusion and exclusion of features based on user-defined significance thresholds.
- Optional specification of optimization method for model fitting.
- Optional inclusion of interaction terms for enhanced model complexity.

This library is suitable for data scientists, researchers, and practitioners working with regression problems who seek a streamlined approach to feature selection. The library intelligently adapts to the nature of the target variable, supporting both linear and logistic regression models, and allows for customization in the regression fitting process.

## Documentation & Examples
For documentation and usage examples, visit the GitHub repository: https://github.com/knowusuboaky/backwards_regression-0.2.0 \
Author: Kwadwo Daddy Nyame Owusu - Boakye\
Email: kwadwo.owusuboakye@outlook.com\
License: MIT

