# Image_Restoration
Image restoration is one of the most important areas in imaging science. Model-based optimization methods and discriminative learning methods have been the two dominant strategies for solving various inverse problems in low-level vision. This paper aims to train different set of images on different models for denoising and deblurring. For denoising salt pepper and Gaussian Noise is introduced in the datasets, and for deblurring Gaussian Blur is used to train the model using CNN(Convolutional Neural Network) and Autoencoders on different datasets. This papers uses the metrics Accuracy, PSNR and SSIM. Experimental results show that Autoencoders in case of salt pepper denoising,  in case of gaussian noise and CNN(Convolutional Neural Network) in case of Gaussian Deblurring gives better results.
<br/>
# Dataset
The link of the dataset used for denoising and deblurring is: https://drive.google.com/drive/folders/1rBxspGhADY_40jWQ5JZ9jtljWF_zryXd?usp=sharing
<br/>
# Conclusion
After running our dataset through different models, we saw that only few models shows the best result in each section. This section contains the final model for Denoising and Deblurring respectively.
<br/>
We performed Denoising on two different types of noises, Salt & Pepper and Gaussian Noise and Deblurring on Gaussian Blur.
## Denoising
### Salt and Pepper Noise
For Salt and Pepper Noise, Autoencoders turned out to be the best fit. The dataset used contains 51 images. This dataset was created by inducing salt-pepper noise randomly all over. 
PSNR of 33.14 in case of Autoencoders was quite satisfactory as compared to the other models, and SSIM of 0.926 was also good. 
We got the desirable results of denoising Salt and Pepper Noise by the Autoencoders Model. The results for the same are shown in the figure 1.
<br/>
![S P_Acc (1)](https://user-images.githubusercontent.com/88244007/140639361-f526c75d-072c-4d0a-8915-d814417f748f.png)
![download](https://user-images.githubusercontent.com/88244007/140639375-8e2e96a5-73fc-4b80-9b41-cbceff0826ff.png)
</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Figure 1:  Salt and Pepper Noise on Autoencoders
<br/>
The above graphs shows the Accuracy vs Epoch and Loss vs Epoch respectively for the Autoencoders Models. 
Below are the images before and after running the model. One can see the different between the noisy image, denoised image and the ground truth respectively.
<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![set3 n](https://user-images.githubusercontent.com/88244007/140645000-66dad885-b48b-4e53-a1e8-431699d177bd.png)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![set3 d](https://user-images.githubusercontent.com/88244007/140645010-d918c397-52f5-4559-b859-ab8ee11e33f5.png)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![set3 g](https://user-images.githubusercontent.com/88244007/140645040-24e5c4c0-3022-4a6f-94f6-bb53b884f82f.png)
<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![set1 noisy (2)](https://user-images.githubusercontent.com/88244007/140645769-07e7b961-a657-4244-b641-666dc340bef2.png)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![set1 predictr](https://user-images.githubusercontent.com/88244007/140646105-bc5a36dc-d927-4ffc-9ce1-af6ccc47a2d3.png)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![set 1 ground truthr](https://user-images.githubusercontent.com/88244007/140646117-08337342-b573-43bc-97ce-263771b10844.png)

Figure 2:  Noisy Image, Denoised Image, Ground Truth respectively for the Autoencoders Model of Salt and Pepper Noise
<br/>

### Gaussian Noise
...content<br>
...figure-3<br>
...figure-4<br>
<hr>

## Deblurring
### Gaussian Blur
For Gaussian Blur, CNN(Convolutional Neural Network) Model turned out to be the best fit. The dataset used contains 51 images and was created by inducing Gaussian Blur randomly all over. Validation PSNR of 34.73 and Training PSNR of 35.57 in case of CNN(Convolutional Neural Network) Model was quite satisfactory as compared to the other models. Hence, as we got fairly satisfactory results from our CNN(Convolutional Neural Network) Model, it is our desired Model for Gaussian Blur Deblurring. The results for the same are shown in the figure given below.<br>
<img width="450" alt="LOSS" src="https://user-images.githubusercontent.com/79861528/140653417-8ca8d847-0714-4ee1-9b91-b1af94a4df10.png">
<img width="442" alt="PSNR" src="https://user-images.githubusercontent.com/79861528/140653454-0fec7508-39a2-4ddc-8a67-0c7469f8307e.png"><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Figure 3:  Gaussian Deblurring using CNN Model<br><br>
The above graphs show the ’Loss vs Epochs’ and ’PSNR vs Epochs’ respectively for CNN(Convolutional Neural Network) Model.<br><br>
<p align="center">
<img width="720" align="center" alt="Screen Shot 2021-11-07 at 8 41 05 PM" src="https://user-images.githubusercontent.com/79861528/140653728-f77ecf3b-453a-4ccc-ad67-3f96b18856cd.png"><br>
</p>
<p align="center">
<img width="722" align="center" alt="AEP5" src="https://user-images.githubusercontent.com/79861528/140653808-5b3763b4-5a84-40ab-894c-24c5b7b45ec2.png"><br>
</p>
Figure 4:  Input(Blurred), Ground Truth and Predicted(Deblurred) images respectively for the CNN Model for Gaussian Blur.
<br><br>

Above are the images of the Input(Blurred), Ground Truth and Predicted(Deblurred) images using the CNN model for Gaussian Deblurring of the images.
