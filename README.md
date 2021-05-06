# NoiseFiltering
Studying the effect of different filters on different kinds of noise added to an image

Q1. How does Mean filter effect the image quality, discussing effect of filter size? 

Ans1.
What mean filter does is , with the given kernel size, it creates windows, takes the intensity values of those individual kernels in the window and calculates a mean value which is then used to replace the geometrical centre kernel of the window The window is moved around the whole image, the same procedure is followed, and thereby filtering is done.
We see that Gaussian noise remains after mean filtering. Mean filter is evidently not ideal for Gaussian noise and we see that with larger kernel size, more blurring happen, which is also obvious, taking into account the working principle of Mean Filter.
we see that Salt & Pepper  noise remains after mean filtering. Mean filter is evidently not ideal for Salt & Pepper noise and we see that with larger kernel size, more blurring happen, which is also obvious, taking into account the working principle of Mean Filter.


 
Q2. How does Median filter effect the image quality, discussing effect of filter size? 

Ans2.

What median filter does is, with the given kernel size, it creates windows, takes the intensity values of those individual kernels in the window, arranges them in an ascending order and calculates the central value which is then used to replace the geometrical centre kernel of the window. The window is moved around the whole image, the same procedure is followed, and thereby filtering is done.
we see that Gaussian noise remains after median filtering. Median filter is evidently not ideal for Gaussian noise and we see that with larger kernel size, more blurring happen, which is also obvious, taking into account the working principle of Median Filter. On Gaussian noise, Mean and Median filters almost have a similar effect.
we see that Median Filter, filters out Salt and Pepper noise very very efficiently. A smaller kernel size is preferable as a larger kernel size evidently blurs out features of the image which causes loss in data.


Q3. How does Gaussian filter effect the image quality, discussing effect of filter size & standard deviation? 

Ans3.

Gaussian filter works by using a 2D distribution function which is convolved with the image.
It is a non uniform LPF. The kernel Co-efficients diminish with increasing distance from the kernel centre. Also, central pixel have higher weighting than those on the periphery.
This kind of filter might not preserve image brightness and most of the times lead to image blurring.
we see that Gaussian filter does not very effectively remove  the Gaussian noise, which is justified because the work of the Gaussian filter is not to remove noise selectively, rather it is to smoothen and/or blur images. It is so due to the way the filter works. 
Here we see that the Gaussian filter doesn’t remove the salt &pepper noise, moreover, it also slightly blurs the image. This is justified by the working principle of the filter.
Regarding the kernel size,
For Gaussian noise, the smaller kernel seems to have better sharpness, albeit the visible difference is very minimal.
Same is the case for Salt & Pepper Noise. A smaller kernel size gives better sharpness.
The measure for that is gotten from peak SNR.


 
Q4. Which filter is best for Salt and pepper noise and why? 

Ans4. Median Filter, filters out Salt and Pepper noise very effectively. This is attributed to the working principle of Median Filter.

What median filter does is, with the given kernel size, it creates windows, takes the intensity values of those individual kernels in the window, arranges them in an ascending order and calculates the central value which is then used to replace the geometrical centre kernel of the window. The window is moved around the whole image, the same procedure is followed, and thereby filtering is done.
Median filter is best to filter out noise which are extreme in nature, as this filter does not do averaging, rather it removes the extreme intensity values.



Q5. Which filter is best for Gaussian noise and why? 

Ans5. Gaussian noise is a noise which has a PDF equal to a normal distribution
Gaussian noise can be filtered using spatial filters (Mean, Gaussian filters).
Although, spatial filters, while smoothening may blur out data as they block high frequencies.
The Kernel size must be optimised for the particular file type. Also, the performance of different kernel size could be checked using peak snr values.

