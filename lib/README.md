# Project: Can you unscramble a blurry image? 

# Libraries folder
This folder contains all the functions used in *main.rmd*
+ `feature.R` defines the function I used to extract features from images
+ `evalution.R` defines the function used to calculate MSE and PSNR of test images
+ `cross_validation.R` defines the function used to calculate CV errors which are used for model selection
+ `super_revolution.R` defines the function used to generate predicted images using GBM
+ `test.R` defines the function used to predict image matrix in cross validation section
+ `train.R` defines the function used to train GBM model using training images data

The files end with **parallel** use parallel comupting for shortening training time and have same function as non-parallel ones.

# SRGAN
The [SRGAN](https://github.com/TZstatsADS/Spring2019-Proj3-grp12/tree/master/lib/SRGAN) folder contains four file which defines the model.

[main.py](https://github.com/TZstatsADS/Spring2019-Proj3-grp12/blob/master/lib/SRGAN/main.py) defines the `train` and `predict` function.

[model.py](https://github.com/TZstatsADS/Spring2019-Proj3-grp12/blob/master/lib/SRGAN/model.py) defines the `generater`, `discriminator` and `vgg19` model.

[utils.py](https://github.com/TZstatsADS/Spring2019-Proj3-grp12/blob/master/lib/SRGAN/utils.py) defines `cropping` and `downsampling` function.

[vgg19.npy](https://github.com/TZstatsADS/Spring2019-Proj3-grp12/blob/master/lib/SRGAN/vgg19.npy) is the pre-trained `VGG19` model.
