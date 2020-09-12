# BERT-DST

Contact: Guan-Lin Chao (guanlinchao@cmu.edu)

Source code of our paper [BERT-DST: Scalable End-to-End Dialogue State Tracking with Bidirectional Encoder Representations from Transformer](https://arxiv.org/abs/1907.03040) (Interspeech 2019).
```
@inproceedings{chao2019bert,
title={{BERT-DST}: Scalable End-to-End Dialogue State Tracking with Bidirectional Encoder Representations from Transformer},
author={Chao, Guan-Lin and Lane, Ian},
booktitle={INTERSPEECH},
year={2019}
}
```

Tested on Python 3.6, Tensorflow==1.13.0rc0

## Install required packages

```
## Create a virtual environment (optional but recommended)
python3.6 -m venv venv
source venv/bin/activate

pip install tensorflow==1.13.0rc0
pip install tensorflow_estimator==1.13.0rc0
```

## Additional requirements (no need to install, just provide the paths in code)
1. [bert](https://github.com/google-research/bert)
2. uncased_L-12_H-768_A-12: pretrained [BERT-Base, Uncased] model checkpoint. Download link in [bert](https://github.com/google-research/bert).

## Datasets
dstc2-clean, woz_2.0, [sim-M and sim-R](https://github.com/google-research-datasets/simulated-dialogue)

## Usage

* Check the directory paths in `train.sh`, `eval_pred.sh`, `main.py`, and `dataset_dstc2.py`
* Run `./train.sh` to train the model
