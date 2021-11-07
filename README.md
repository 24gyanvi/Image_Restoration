# Image_Restoration
Image restoration is one of the most important areas in imaging science. Model-based optimization methods and discriminative learning methods have been the two dominant strategies for solving various inverse problems in low-level vision. This paper aims to train different set of images on different models for denoising and deblurring. For denoising salt pepper and Gaussian Noise is introduced in the datasets, and for deblurring gaussian blur is used to train the model using CNN(Convolutional neural network) and autoencoders on different datasets. This papers uses the metrics accuracy, PSNR and SSIM. Experimental results show that Autoencoders in case of salt pepper denoising,  in case of gaussian noise, in case of deblurring gives the better results.
<br/>
# Dataset
The link of the dataset used for denoising and deblurring is: https://drive.google.com/drive/folders/1rBxspGhADY_40jWQ5JZ9jtljWF_zryXd?usp=sharing
<br/>
# Conclusion
After running our dataset through different models, we saw that only few models shows the best result in each section. This section contains the final model for denoising and deblurring respectively.
<br/>
We performed denoising on two different types of noises, salt & pepper and Gaussian Noise.
## Salt and Pepper Noise
For salt and pepper noise, Autoencoders turned out to be the best fit. The dataset used contains 51 images. This dataset was created by inducing salt-pepper noise randomly all over. 
PSNR of 33.14 in case of autoencoders was quite satisfactory as compared to the other models, and SSIM of 0.926 was also good. 
We got the desirable results of denoising salt and pepper noise by the Autoencoders model. The results for the same are shown in the figure 1.
<br/>
![S P_Acc (1)](https://user-images.githubusercontent.com/88244007/140639361-f526c75d-072c-4d0a-8915-d814417f748f.png)
![download](https://user-images.githubusercontent.com/88244007/140639375-8e2e96a5-73fc-4b80-9b41-cbceff0826ff.png)
</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Figure 1:  Salt and Pepper Noise on Autoencoders
<br/>
The above graphs shows the Accuracy vs Epoch and Loss vs Epoch respectively for the autoencoders models. 
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

Figure 2:  Noisy image, denoised image, ground truth respectively for the Autoencoders model of salt and pepper noise
<br/>
