# WGAN and DCGAN over FashionMNIST


In this notebook we first implement the network proposed for CIFAR-10 in ["Improved Training of Wasserstein GANs"](https://arxiv.org/abs/1704.00028) by Gulrajani et al. More precisely, we will replicate the simpler architecture used for CIFAR10 (see references) and train it on FashionMNIST. The necessary adaptations will be detailed below.

We will also implement a [DCGAN](https://arxiv.org/pdf/1511.06434.pdf) and compare the performance of both networks.


References:
- The original code (using TensorFlow): the [simpler version](https://github.com/igul222/improved_wgan_training/blob/master/gan_cifar.py). There is also a [residual version](https://github.com/igul222/improved_wgan_training/blob/master/gan_cifar_resnet.py), which is not implemented here.
- A [suggested network for MNIST](https://github.com/igul222/improved_wgan_training/blob/master/gan_mnist.py) by the authors, which we took inspiration from. 
- The WGAN-GP [implementation](https://github.com/EmilienDupont/wgan-gp/blob/master/models.py) by Emilien Dupont.
- The WGAN-GP [implementation](https://github.com/caogang/wgan-gp/blob/master/gan_cifar10.py) by Marvin Cao.
- The [DCGan PyTorch tutorial on Celeb-A](https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html) by Nathan Inkawhich.