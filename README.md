# Multi-task Learning with Sample Re-weighting for Machine Reading Comprehension

This PyTorch package implements the Multi-Task Stochastic Answer Network (MT-SAN) for Machine Reading Comprehension, as described in:

Yichong Xu, Xiaodong Liu, Yelong Shen, Jingjing Liu and Jianfeng Gao<br/>
Multi-task Learning with Sample Re-weighting for Machine Reading Comprehension</br>
North American Chapter of the Association for Computational Linguistics (NAACL), 2019<br/>
[arXiv version](https://arxiv.org/abs/1809.06963)

Please cite the above paper if you use this code. 

## Results
We report single-model results produced by this package as follows.

| Dataset | EM/F1 | 
| ------- | ------- | 
| `SQuAD v1.1` (Rajpurkar et al., 2016) | **81.6**/**88.2** (development set) |
| `NewsQA` (Trischler et al., 2016)| **59.9**/**72.6** (vs. 46.5/69.4 Human Performance)|

## Quickstart 

#### Install via pip:
1. python3.6

2. install requirements </br>
   ```> pip install -r requirements.txt```

#### Use  docker:
1. pull docker: We can use the same docker as [mt-dnn](https://github.com/namisan/mt-dnn) </br>
   ```> docker pull allenlao/pytorch-mt-dnn:v0.1```

2. run docker </br>
   ```> docker run -it --rm --runtime nvidia  allenlao/pytorch-mt-dnn:v0.1 bash``` </br>
    Please refer to the following link if you first use docker: https://docs.docker.com/


#### Train a MT-SAN Model
1. prepare data
   > ./prepare_data.sh
2. train a model: See example codes in [run.sh](https://github.com/xycforgithub/MultiTask-MRC/blob/master/run.sh)

#### Pretrained Models
You can download pretrained models with the best SQuAD performance [here](https://microsoft-my.sharepoint.com/:u:/p/yicxu/EcMFiMsPJgVMkfKGMjFg44gBkjr2v7yLOrvGMXTVhcopOQ?e=Qq2S6x).

## Notes and Acknowledgments
The code is developed based on the original SAN code: https://github.com/kevinduh/san_mrc

Related: <a href="https://arxiv.org/abs/1901.11504">MT-DNN</a>

by
yichongx@cs.cmu.edu




