# Learning to See in the Dark

# Presented by
yt2188@nyu.edu – Yash Thesia
ms12418@nyu.edu – Meera Suthar

# Abstract

Image data has become a crucial part of daily life. The image quality depends on parameters such as bad weather, electrical noise, poor lighting, camera quality, etc. The obvious solution here is to perform image preprocessing before feeding images to any network, but sometimes that leads us to noisy, blurry, color-shifted images. There has been significant progress in Convolution-based Deep Learning models in the Computer Vision domain which solve many challenging issues such as Image Denoising, Image Restoration, Image Segmentation, and Detection. While solving low-light image-related issues, a Convolutional model can give us promising results as we need to add the features while still maintaining image size and shape. We proposed an Attention U-Net GAN model architecture that makes use of supervised learning using the See-in-the-Dark (SID) dataset and enhances low light images. Attention U-Net is useful to highlight dark spots in the images and GAN learns high-level image enhancement loss automatically and produces a brighter image. We compared our results with other benchmark techniques and received improved peak signal-to-noise-ratio (PSNR) and SSIM values.


## Results
|                   | PSNR on test set | 
|-------------------|------------------|
| Chen et al.       | 27.60            | 
| My implementation | 28.96            | 

- Results and Comparisons (All the models were trained for only 500 epochs; increasing the number of epochs for training may increase the resultant PSNR and SSIM values)

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

- [1] https://github.com/huyvnphan/Learning_To_See_In_The_Dark
- [2] https://github.com/LeeJunHyun/Image_Segmentation
- [3] https://github.com/ozan-oktay/Attention-Gated-Networks
- [4] https://github.com/aladdinpersson/Machine-Learning-Collection/tree/master/ML/Pytorch/GANs
- [6] Isola, P., Zhu, J. Y., Zhou, T., & Efros, A. A. (2017). Image-to-image translation with conditional adversarial networks. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 1125-1134).
- [7] Chen Chen, Qifeng Chen, Jia Xu, and Vladlen Koltun. Learning to see in the dark. 2018 IEEE/CVF Conference on Computer Vision and Pattern Recognition, pages 3291–3300, 2018. 2, 3, 4
