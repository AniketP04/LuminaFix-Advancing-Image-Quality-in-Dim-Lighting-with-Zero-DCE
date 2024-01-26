# Zero-Reference Low-Light Image Enhancement

Low-light image enhancement aims to raise the quality of pictures taken in dim lighting, resulting in a brighter, clearer, and more visually appealing image without adding too much noise or distortion. One of the state-of-the-art methods for this computer vision task is Zero-DCE. This method uses just a low-light image without any image reference to learn how to produce an image with higher brightness. There are four loss functions crafted specifically for this zero-reference low-light image enhancement method, i.e., color constancy loss, exposure loss, illumination smoothness loss, and spatial consistency loss.

## Result

## Quantitative Result

The quantitative performance of the model is exhibited in the table below.

Metrics | Test Dataset |
------------ | ------------- |
Color Constancy Loss |  0.065 |
Exposure Loss | 0.391 |
Illumination Smoothness Loss | 0.094 |
Spatial Consistency Loss | 0.042 |
Total Loss | 0.592 |
PSNR | 13.646 |
SSIM | 0.663 |
MAE | 0.170 |


## Evaluation Metrics Curve

<p align="center"> <img src="https://github.com/AniketP04/LuminaFix-Advancing-Image-Quality-in-Dim-Lighting-with-Zero-DCE/blob/main/assets/colorconstancy_loss_curve.png" alt="colorconstancy_loss_curve" > <br /> Color constancy loss curve on the train set and the validation set. </p>

<p align="center"> <img src="https://github.com/AniketP04/LuminaFix-Advancing-Image-Quality-in-Dim-Lighting-with-Zero-DCE/blob/main/assets/exposure_loss_curve.png" alt="exposure_loss_curve" > <br /> Exposure loss curve on the train set and the validation set. </p>

<p align="center"> <img src="https://github.com/AniketP04/LuminaFix-Advancing-Image-Quality-in-Dim-Lighting-with-Zero-DCE/blob/main/assets/illumination_smoothness_loss_curve.png" alt="illumination_smoothness_loss_curve" > <br /> Illumination smoothness loss curve on the train set and the validation set. </p>

<p align="center"> <img src="https://github.com/AniketP04/LuminaFix-Advancing-Image-Quality-in-Dim-Lighting-with-Zero-DCE/blob/main/assets/spatialconsistency_loss_curve.png" alt="spatialconsistency_loss_curve" > <br /> Spatial consistency loss curve on the train set and the validation set. </p>

<p align="center"> <img src="https://github.com/AniketP04/LuminaFix-Advancing-Image-Quality-in-Dim-Lighting-with-Zero-DCE/blob/main/assets/totalloss_curve.png" alt="totalloss_curve" > <br /> Total loss curve on the train set and the validation set. </p>

<p align="center"> <img src="https://github.com/AniketP04/LuminaFix-Advancing-Image-Quality-in-Dim-Lighting-with-Zero-DCE/blob/main/assets/psnr_curve.png" alt="psnr_curve" > <br /> PSNR curve on the train set and the validation set. </p>

<p align="center"> <img src="https://github.com/AniketP04/LuminaFix-Advancing-Image-Quality-in-Dim-Lighting-with-Zero-DCE/blob/main/assets/ssim_curve.png" alt="ssim_curve" > <br /> SSIM curve on the train set and the validation set. </p>

<p align="center"> <img src="https://github.com/AniketP04/LuminaFix-Advancing-Image-Quality-in-Dim-Lighting-with-Zero-DCE/blob/main/assets/mae_curve.png" alt="mae_curve" > <br /> MAE curve on the train set and the validation set. </p>


## Qualitative Result

Here are some samples of the qualitative results of the model.

<p align="center"> <img src="https://github.com/AniketP04/LuminaFix-Advancing-Image-Quality-in-Dim-Lighting-with-Zero-DCE/blob/main/assets/enhancement_qualitative_00.png" alt="enhancement_qualitative_00" > <br /> <img src="https://github.com/AniketP04/LuminaFix-Advancing-Image-Quality-in-Dim-Lighting-with-Zero-DCE/blob/main/assets/enhancement_qualitative_01.png" alt="enhancement_qualitative_01" > <br /> <img src="https://github.com/AniketP04/LuminaFix-Advancing-Image-Quality-in-Dim-Lighting-with-Zero-DCE/blob/main/assets/enhancement_qualitative_02.png" alt="enhancement_qualitative_02" > <br /> The qualitative results of the image enhancement method (comparing the original, the ground-truth, the PIL autocontrast, and the prediction). </p>


## Reference

- [(Paper) Zero-Reference Deep Curve Estimation for Low-Light Image Enhancement](https://arxiv.org/pdf/2001.06826.pdf)
- [PyTorch Lightning](https://lightning.ai/docs/pytorch/latest/)
