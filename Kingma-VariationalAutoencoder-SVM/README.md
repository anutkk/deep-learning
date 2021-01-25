# Feature extraction using Variational Autoencoder

In this part we implement the paper "[Semi-supervised Learning with Deep Generative Models](https://papers.nips.cc/paper/5352-semi-supervised-learning-with-deep-generative-models.pdf)" by Kingma et al. We focus on the M1 algorithm.

The basic idea is to train a variational autoencoder (VAE), then use the encoder only to extract features and train a classifier (here, a SVM) on the features.