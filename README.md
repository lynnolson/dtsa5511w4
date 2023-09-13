# dtsa5511w4

week 4 assignment for DTSA5511

<!-- ABOUT THE PROJECT -->
## About the assignment
This project applies RNNs to classify whether a tweet is related to a natural disaster or not. It's the Kaggle task [NLP Disaster Tweets](https://www.kaggle.com/competitions/nlp-getting-started/).

It was done for CU Boulder's DTSA5511 Introduction to Deep Learning.

The models developed include
- BiLSTMs
- BiGRUs
  
Both of course are RNN-based models.

Hyperparameter searching was done with [Weights and Biases](https://wandb.ai/site).

### Dependencies

The code was developed with Python 3.10.4 and the following libraries and versions:

- nltk==3.8.1
- numpy==1.24.3
- pandas==2.0.3
- sklearn==1.3.0
- torch==2.0.1+cu117
- torchtext==0.15.2
- wandb==0.15.9

You will need a [Weights and Biases](https://wandb.ai/site) account.

The full environment setting can be installed through:
```
conda env create -f conda-environment.yaml
conda activate msds
```

### Data

The [data](https://www.kaggle.com/competitions/nlp-getting-started/data) used was downloaded from Kaggle.  I don't include it here because you have to read and agree to Kaggle's rules before using their data.

### Usage

All code may be found and run in the notebook nlp_dist_tweet.ipynb.  The models were trained on a A100 GPU with 48GB of memory. They can be trained on something much, much smaller but would likely still need a GPU.
