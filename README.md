# LMLFM
This is a python implementation of Longitudinal Multi-Level Factorization Machines (LMLFM) in the following paper:

Junjie Liang, Dongkuan Xu, Vasant Honavar. Longitudinal Multi-Level Factorization Machines, *ICML'2019* (under review)

## Short description

LMLFM extends FM to handle fixed, random, or mixed effects as needed for predictive modeling from longitudinal data. In addition, LMLFM incorporates a small but important change to the way latent factors are associated with the observations that not only enhances the interpretability of the resulting predictive model but also being more efficient with computational complexity strictly linear to the size of training data. For full description, please refer to our paper.

## Usage

### Requirements

* python 3.x (Recommend Anaconda)
* numpy, pandas, scipy, sklearn
* statsmodels.stats
* numba

### Format of Input Data

Please find the example of training data in [train.csv](train.csv). Basically, each line is a training sample, which is constructed by a vector of features, an individual id (`iid`), an observation id (`oid`) and a label (`label`).

### Demo

Please follow the code in [UseCase](UseCase.ipynb).

## Contacts

Please contact me through email <jul672@ist.psu.edu> for any question. 