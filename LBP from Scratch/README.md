# LBP

## Steps:

* Load the image and convert it into gray.
* Divide the examined image into cells of 3X3 known as patch.
* For each pixel in a patch, compare pixels into it’s each neighbour (on its left-top, leftmiddle, left-bottom, right-top).
* Where the center pixel value is greater than neighbour value put 1 otherwise 0. Thenconvert those numbers to 8-digit binary number by following the circle either clockwise or anticlockwise.
* Apply this algorithm on another image also.
* Then, compare each patch of one image with all the patches of other image recursively.
* Find the index of matching pattern and show those matching patch of a inital image.
