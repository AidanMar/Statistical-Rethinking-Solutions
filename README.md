# Statistical-Rethinking-Solutions
The Systems and Signals group at Imperial College London is doing a reading group based on Richard McElreath's book, Statistical Rethinking. The book is a great primer to bayesian inference and performing data analysis in code.

Here I present some a set of solutions to the end of chapter problems. The solutions are implemented in python, primarily making use of PyMC3, a probabilistic programming language, well suited for doing bayesian analysis in a straightforward manner.

# Install

## Using my environment

If you're using anaconda, you can download: <a href="https://github.com/AidanMar/Statistical-Rethinking-Solutions/blob/main/Bayes.yml" download="Bayes.yml">Bayes.yml</a>

This yml contains a bunch of packages like pymc3, graphviz, causalgraphicalmodels, and a few others that will be helpful along the way as you work your way through the book.

Once downloaded use this command to install the conda environment:

```conda env create -f Bayes.yml```

 If you're running on Linux or mac OS X I'd recommend taking the time to setup theano, and make sure that your command line has g++ installed which can compile c++ code.  Whilst not essential, doing this will make pymc3 run much (MUCH!) faster, as it will use c++ to perform Markov Chain Monte Carlo (MCMC). Without having a c-compiler, pymc3 will instead use numpy perform MCMC, which is unbearably slow. 

If you're using windows, in the immortal words of Obi-Wan-Kenobi "You want to go home and rethink your life".

## Using pip

If the above environment doesn't work, then enter the following into your command line

``` pip install pymc3```

# NB

The notebooks are all still works in progress, and "copy editing" has yet to be done. So don't be too harsh/judgy about all of the typos and grammatical errors
