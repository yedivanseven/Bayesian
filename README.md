# Bayesian
## Bayesian Perambulations

This repository contains applications of Bayesian Monta-Carlo methods. So far,
there are two tried-and-tested examples:

+ Coin Toss
+ Linear Regression

## Dependencies and Install
Everything seems to run smoothly on a fresh Anaconda 4.3 install (under
`python 3.6`). Additional dependencies are

 + `pymc 2.3.6`

and, if you want to plot the graph corresponding to your Bayesian model,
you will need also:

 + `pydotplus 2.0.2`
 + `graphviz 2.38`

Note that `pymc` actually depends on `pydot`, which is not,
however, compatible with fresher python versions. The package `pydotplus` was
written to overcome that problem. In order for `pymc` to use it, simply change
the line

`import pydot`

in the header of the `graph.py` module of `pymc` to:

`import pydotplus as pydot`
