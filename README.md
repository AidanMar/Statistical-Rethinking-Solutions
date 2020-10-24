# Statistical-Rethinking-Solutions
The Systems and Signals group at Imperial College London is doing a reading group based on Richard McElreath's book, Statistical Rethinking. The book is a great primer to bayesian inference and performing data analysis in code.

Here I present some a set of solutions to the end of chapter problems. The solutions are implemented in python, primarily making use of PyMC3, a probabilistic programming language, well suited for doing bayesian analysis in a straightforward manner.

# Install
If you're using anaconda, you can download: <a href="https://github.com/AidanMar/Statistical-Rethinking-Solutions/blob/main/Bayes.yml" download="Bayes.yml">Bayes.yml</a>

Once downloaded use this command to install the conda environment:

conda env create -f Bayes.yml

This yml contains a bunch of packages like pymc3, graphviz, causalgraphicalmodels, and a few others that will be helpful along the way. If you're running on Linux or macOSX I'd recommend taking the time to setup theano, and make sure that your command line has g++ installed which can compile c++ code. Whilst not essential, doing this will make pymc3 run much (MUCH!) faster, as it will use c++ to perform Markov Chain Monte Carlo (MCMC). Without having a c-compiler, pymc3 will instead use numpy perfoorm MCMC, which is unbearably slow.
