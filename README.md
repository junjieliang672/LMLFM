# Mix-FM
This is a python implementation of Mix-FM in the following paper:

Junjie Liang, Dongkuan Xu, Vasant Honavar. Mix-FM: A Factorization Machine for Predictive Modeling from High Dimensional Longitudinal Data, *ICML'2019* (under review)

## Short description

Mix-FM is adapted from Factorization machines (FM) to handle longitudinal data. It extends FM to avoid the need for tunable hyperparameters, handle fixed, random, or mixed effects as needed for predictive modeling from longitudinal data. For full description, please refer to our paper.

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