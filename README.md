## Solution to the bin bag classification task

1. Detecting the bags

The detecting_bags jupyter notebook shows the work done to detect the bags on the images. The method is based on using pixel value differences between images with bags and ones without bags. 143 out of the 144 bags are detected correctly.
<br>
This notebook also serves to save the detected bags under the form of rescaled 50x50x3 pixels images. This allows to have all the bags as same sized images and provides the features for the next step.

2. Classyfing the bags

The PCA_SVM jupyter notebook serves to classify each bag detected. A cross-validation is performed along with data aumentation (rotation and horizontal & vertical flips) providing a final mean accuracy of 0.80. 
