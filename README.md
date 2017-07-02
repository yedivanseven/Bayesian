# Bayesian
### Bayesian Perambulations

This repository explores concepts of Bayesian Monte-Carlo methods. If you are more interested in realistic applications of probabilistic models, check out the
_Bayesian_ notebook in the [_Commodities_](https://github.com/yedivanseven/Commodities) repository
or the _PlanBayesian_ notebook in the [_Berlin_](https://github.com/yedivanseven/Berlin) repository.

## 1. Coin Toss
In this notebook, we play with what may well be the simplest of all probabilistic models.

#### Specific dependendencies
This notebook still runs on
+ `pymc 2.3.6`

and, if you want to plot the graph corresponding to your Bayesian model,
you will need also:

+ `pydotplus 2.0.2`
+ `graphviz 2.38`

## 2. Linear Regression
In this notebook, Monte-Carlo results are critically examined and compared to the known analytic solution for the Gauss - InverseGamma Model.

#### Specific dependendencies
This notebook still runs on
+ `pymc 2.3.6`

and, if you want to plot the graph corresponding to your Bayesian model,
you will need also:

+ `pydotplus 2.0.2`
+ `graphviz 2.38`

## 3. Model Selection
Here, we explore the possibility of re-using Monte-Carlo samples to actually compute the Bayes-factors between two models and, thus, decide which one to pick to describe our data.

#### Specific dependendencies
This notebook now runs on
+ `pymc 3.1`

which has `theano 0.9` as a dependency.

## General Dependencies
Everything seems to run smoothly on a fresh Anaconda 4.3 install (under `python 3.6`).

Note that `pymc 2.3.6` actually depends on `pydot`, which is not,
however, compatible with fresher python versions. The package `pydotplus` was
written to overcome that problem. In order for `pymc 2.3.6` to use it, simply change
the line

`import pydot`

in the header of the `graph.py` module of `pymc` to:

`import pydotplus as pydot`
