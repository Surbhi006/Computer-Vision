# HOG Feature Extraction

## Steps:

* First Load the dataset and convert into gray.
* Apply a vertical edge and horizontal detection filter to obtain vertical edge map and horizontal edge map.
* Intialize magnitude and array of same size as that of image.
* Compute gradient angle and magnitude.
* Divide the image into patches.
* Initialize the bins another array hog of shape patches and bins.
* Comute histogram over a patch that accumulates the magnitudes of the pixels in the patch using key angles as bins.
* Divide the magnitude of a pixel depending upon the proximity of the angle of the pixel to the nearest key angles.
* Once magnitudes of all the pixels in the patch are accumulated, we have this histogram as feature vector of the patch.
* Concatenate the HOG features of all the patches to generate feature for an image.
* On resulting images, apply SVM using sklearn and classify images.
* At last find accuracy with test and predicted y.
