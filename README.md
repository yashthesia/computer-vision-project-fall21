# Learning to See in the Dark
This is my Pytorch implementation of Learning to See in the Dark in CVPR 2018. For more information, please read the Report.pdf and See-In-The-Dark notebook.


[Original paper](http://cchen156.web.engr.illinois.edu/paper/18CVPR_SID.pdf) by [Chen Chen](http://cchen156.web.engr.illinois.edu/), [Qifeng Chen](http://cqf.io/), [Jia Xu](http://pages.cs.wisc.edu/~jiaxu/), and [Vladlen Koltun](http://vladlen.info/).

[Original Tensorflow implementation](https://github.com/cchen156/Learning-to-See-in-the-Dark) by Chen Chen

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
