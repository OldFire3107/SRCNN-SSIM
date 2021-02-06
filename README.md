# SRCNN-SSIM
We have put together an implementation of SRCNN with SSIM cost in pytorch. 

### How it Works

An image is changed from RGB to YCbCr colour scheme. The image is scaled by Bicubic Interpolation. It is then passed through a SRCNN, trained for 400 epochs with SSIM (Structural Similarity) as the cost function, which produces a sharper image. The sharper image is change from YCbCr to RGB color scheme.

Please read the comments for a deep understanding of the functioning.

### Results

---> Original Image

![](./images/zebra.bmp)

---> Bicubic Interpolation Output (4x Upscaled and Downscaled)

![](./images/zebra_bicubic_x4.bmp)

---> SRCNN Output (4x Upscaled)

![](./images/zebra_final_x4.bmp)

---> SRCNN Output (4x Upscaled and Downscaled)

![](./images/zebra_srcnn_x4.bmp)