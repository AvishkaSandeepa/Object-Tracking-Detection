# Object Tracking & Detection

This project is about Object Counting on a Convey Belt. When giving the video input of convey belt this alogorithm is able to count the number of nuts on the belt while tracking its details. Then this algorithm will create an output video of a object counting annotation. 

> ***You can simply go through the noteboook while learning. Anyone have an interest can follow each section easily. There are theoritical explanation unser each section.***


Here is the snapshot of the output video...
![Snapshot](https://github.com/AvishkaSandeepa/EN2550-2021-Assignment-05/blob/master/created_video/Capture.PNG)



### Steps

* Open the images as grayscale images
*     Since thresholding needs binary image original one is converted to grayscale
* Thresholding the imnages usin OTSU Thresholding
*     Apart from the conventional simple thresholding techniques, use OTSU thresholding that consider the histogram of the image for best thresholding
* Morphological transformations are done
*     To fulfil the image after thresholding , used Morphological Closing to filling small holes from an image while preserving the shape
* Connected component analysis
*     Find the each connected components with label and outputs the details under each label
* Contour analysis
*     Find the contour for object detection and Contour Drawing for output
* Count the number of matching hexagonal nuts on the belt
*     Using functions, Count the no of nuts and their indexes
* Frame tracking through image moments
*     For each frame calculate the moments of the nuts
* Object Tracking and Detection
*     Using Function, Detect the nuts on the belt and count. Finally store the detection as video
