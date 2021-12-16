# Learning to See in the Dark
This is my Pytorch implementation of Learning to See in the Dark in CVPR 2018. For more information, please read the Report.pdf and See-In-The-Dark notebook.


[Original paper](http://cchen156.web.engr.illinois.edu/paper/18CVPR_SID.pdf) by [Chen Chen](http://cchen156.web.engr.illinois.edu/), [Qifeng Chen](http://cqf.io/), [Jia Xu](http://pages.cs.wisc.edu/~jiaxu/), and [Vladlen Koltun](http://vladlen.info/).

[Original Tensorflow implementation](https://github.com/cchen156/Learning-to-See-in-the-Dark) by Chen Chen

# Presented by
yt2188@nyu.edu – Yash Thesia
ms12418@nyu.edu – Meera Suthar

# Abstract

This term paper surveys various research papers aimed at forecasting weather. We explore cutting-edge research towards deep learning algorithms and technology. Convolutional networks help preserve information of data points in physical or logical proximity when placed together on a matrix, and help reduce the computation size using the concept of 2-D filters, for example precipitation levels of a location based on levels of neighboring cities or towns. Recurrent networks help preserve information gained with past iterations of training, and are thus much more flexible when trying to analyze time-series data, like today’s precipitation levels based on past precipitation levels. And autoencoders help overcome overfitting by extracting useful features from the given data, which also helps reduce the vanishing gradient problem.


## Results
|                   | PSNR on test set | 
|-------------------|------------------|
| Chen et al.       | 27.60            | 
| My implementation | 28.96            | 


## Low Light Image Enhancement Proposed Pipeline 
![Model Architecture](figures/atten_Unet_GAN.png)

## Training & validation PSNR
![Training PSNR and L1 Loss](figures/atten_loss.png)

## Model visual Output Comparision & attenstion weights of last layer
![Denoise a random image in original dataset](figures/results.png)


## Requirements
- 128GB RAM
- Pytorch 1.0
- Numpy + Rawpy
- Matplotlib
- GPU : Nvidia RTX1800

## References 
