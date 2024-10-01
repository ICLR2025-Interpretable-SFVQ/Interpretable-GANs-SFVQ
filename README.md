# Unsupervised Panoptic Interpretation of Latent Spaces in GANs Using Space Filling Vector Quantization
This repository contains the PyTorch implementation of the paper entitled "Unsupervised Panoptic Interpretation of Latent Spaces in GANs Using Space-Filling Vector Quantization" submitted to ICLR 2025.

# demo
This directory contains the demo to test and compare interpretable directions found by our proposed method, GANSpace, and LatentCLR methods in intermediate latent space (W) of StyleGAN2 pretrained on FFHQ dataset. To use the demo, please follow the steps below: 

Please create the conda environment to use this repository using the following lines in your terminal window:

`conda create --name wacv2025_sfvq python=3.9`

`conda activate wacv2025_sfvq`

`pip install -r requirements.txt`

Also, please download the StyleGAN2-FFHQ pretrained model under [this link.](https://drive.google.com/file/d/11nQSxaJJ4RQEZkSCFCC6wntQky4uZZhj/view?usp=sharing)

In addition, please extract the files existing in 'files.zip'. Please keep the pretrained model and extracted files in the same directory as "demo.py".

In 'demo.py' code, you only need to change the "direction_name" and "sigma_list" variables to test interpretable directions over different shift values ($\sigma$).
