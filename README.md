# Unsupervised Panoptic Interpretation of Latent Spaces in GANs Using Space Filling Vector Quantization
This repository contains the PyTorch implementation of the paper entitled "Unsupervised Panoptic Interpretation of Latent Spaces in GANs Using Space-Filling Vector Quantization" submitted to ICLR 2025.

# demo
This directory contains the demo to test and compare interpretable directions found by our proposed method, GANSpace, and LatentCLR methods in intermediate latent space (W) of pretrained StyleGAN2-FFHQ.

**Contents of this directory:**
- `comparison.pdf`: Comparison of our method over 20 random vectors with GANSpace and LatentCLR
- `demo.py`: Code to create "comparison.pdf" file. You only need to change `num_random_samples` and `sigma_list` in the code.
- `demo_one_direction.py`: Code to compare only one direction for one random sample. You only need to change `direction_name` and `sigma_list` in the code.
- `files.zip`: Required files to run the codes. 

To use the demo, please follow the steps below: 

Please create the conda environment to use this repository using the following lines in your terminal window:

`conda create --name iclr2025_sfvq python=3.9`

`conda activate iclr2025_sfvq`

`pip install -r requirements.txt`

Also, please download the StyleGAN2-FFHQ pretrained model under [this link.](https://drive.google.com/file/d/11nQSxaJJ4RQEZkSCFCC6wntQky4uZZhj/view?usp=sharing)
Or you can download the StyleGAN2 pretrained model named "stylegan2-ffhq-1024x1024.pkl" directly from [NVIDIA website.](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/research/models/stylegan2/files)

In addition, please extract the files existing in 'files.zip'. Please keep the pretrained model and extracted files in the same directory as `demo.py`.

In `demo.py` code, you only need to change the `num_random_samples` and `sigma_list` variables to test interpretable directions over different random vectors and shift values ($\sigma$).

To use CUDA, you need GCC 7 or later (Linux) or Visual Studio (Windows) compilers.
