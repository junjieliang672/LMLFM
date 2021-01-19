# LMLFM
This is a pytorch implementation of the following paper:

**Junjie Liang**, Dongkuan Xu, Yiwei Sun, Vasant Honavar. *[LMLFM: Longitudinal Multi-Level Factorization Machine](https://arxiv.org/abs/1911.04062). AAAI'20*

## Short description

LMLFM extends FM to handle non-iid. data with longitudinal and/or cluster correlation. It simultaneously estimates fixed, random effects and performs variable selection in linear time. For full description, please refer to our [paper](https://arxiv.org/abs/1911.04062).

## Usage
This repo contains three important files.

* The file `GeneratingSyntheticData.ipynb` is for generating the simulated data.
* The file `LMLFM.ipynb` is the main implementation of LMLFM.
* The file `train.ipynb` shows an example on using LMLFM on the simulated data.

### Input format

The input data set should be Pandas Dataframe containing four fields:

`iid` -> The unique individual ID. This should be `Int` and start from 0.

`oid` -> The unique observation ID. This should be `Int` and start from 0.

`X` -> The feature vector.

`y` -> The scalar outcome.

See `GeneratingSyntheticData.ipynb` for example.

## Citation
```
@inproceedings{liang2020lmlfm,
  title={LMLFM: Longitudinal Multi-Level Factorization Machine},
  author={Liang, Junjie and Xu, Dongkuan and Sun, Yiwei and Honavar, Vasant},
  booktitle={Proceedings of the AAAI Conference on Artificial Intelligence},
  volume={34},
  number={04},
  pages={4811--4818},
  year={2020}
}
```
Please feel free to contact [Junjie Liang](mailto:jul672@ist.psu.edu) if you have any question.
