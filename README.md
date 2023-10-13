# ImageSynthesis-FC-GAN
This repository contains the code for reproducing the results in the following paper:

Chengcheng Li, Zi Wang, and Hairong Qi, "Fast-converging conditional generative adversarial networks for image synthesis," 25th IEEE International Conference on Image Processing (ICIP), 2018. [[arXiv]](https://arxiv.org/abs/1805.01972)

# Paper Abstract
Building on top of the success of generative adversarial networks (GANs), conditional GANs attempt to better direct the data generation process by conditioning with certain additional information. Inspired by the most recent AC-GAN, in this paper we propose a fast-converging conditional GAN (FC-GAN). In addition to the real/fake classifier used in vanilla GANs, our discriminator has an advanced auxiliary classifier which distinguishes each real class from an extra 'fake' class. The 'fake' class avoids mixing generated data with real data, which can potentially confuse the classification of real data as AC-GAN does, and makes the advanced auxiliary classifier behave as another real/fake classifier. As a result, FC-GAN can accelerate the process of differentiation of all classes, thus boost the convergence speed. Experimental results on image synthesis demonstrate our model is competitive in the quality of images generated while achieving a faster convergence rate.

# Code
The framework of the code is inherited from Keras-GAN (https://github.com/eriklindernoren/Keras-GAN)

The code is tested with the following environment.

Tensorflow 1.12; keras 1.2.2; Python 3.6.8; Pillow 8.0.1

// This code will run FC-GAN on MNIST.

python fcgan_mnist.py


# Citation
If you find this work useful, please cite:

@inproceedings{li2018fast,
  title={Fast-converging conditional generative adversarial networks for image synthesis},
  author={Li, Chengcheng and Wang, Zi and Qi, Hairong},
  booktitle={2018 25th IEEE International Conference on Image Processing (ICIP)},
  pages={2132--2136},
  year={2018},
  organization={IEEE}
}
