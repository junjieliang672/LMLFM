# LMLFM
This is a python implementation of LMLFM in the following paper:

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

Please find the example of training data in [train.csv](train.csv). Basically, each line is a training sample, which is further  constructed by a vector of features, a subject id (`uid`), an observation id (`iid`) and a label (`label`).

### Demo

Please follow the code in [UseCase](UseCase.ipynb).

## Contacts

Please do not hesitate to contact me through email <jul672@ist.psu.edu> if you have questions. 