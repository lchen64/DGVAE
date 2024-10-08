Dirichlet Graph Auto-Encoders
============

A Pytorch implementation of the [Dirchlet Graph Variational Auto-Encoder model (DGVAE)](https://arxiv.org/abs/2010.04408), NIPS 2020.


DGVAE is an end-to-end trainable neural network model for unsupervised learning, generation and clustering on graphs. This code is more related to graph generation.

DGVAE is based on the Variational Graph Auto-Encoder (VGAE):

T. N. Kipf, M. Welling, [Variational Graph Auto-Encoders](https://arxiv.org/abs/1611.07308), NIPS Workshop on Bayesian Deep Learning (2016)

## Requirements
* pytorch 
* python 3.12
* networkx
* scikit-learn
* scipy

## Create Virtual Environment

* conda create -n DGVAE python=3.12
* conda activate DGVAE
* pip install -r requirements.txt

## Run Demo

```bash
python train_generate.py
```

## Model options

--model       default is our_vae(dgvae), others including our_ae(dgae),gcn_vae,gcn_ae
--dataset     default is Erdos_Renyi, others include Ego, Regular, Geometric, Power_Law, Barabasi_Albert
