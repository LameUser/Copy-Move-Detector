# Image Forgery Detection Tool: 


## Discription
This tool helps you to detect image forgery using the SIFT algo, and this is an easy GUI app which will detect and show the abnormalities present in the image. 


## System Design / Architecture

### Steps involved in the process:

1.	First, the SIFT algorithm from the image is used to draw out the key points.
2.	Then, the feature descriptor is drawn out from every key point on the image including 128 dimensional.
3.	The similarities between the descriptors are calculated to specify the resemblance among the descriptors for specifying the potential forgery on the image. 
4.	The basic obstacle in this algorithm is the computational complexity of the matching stage where it is very high because of the big number of key points drawn  out from the image and the matching process amongst them. 
5.	As a result, we use the clustering algorithm for clustering the key points depending on their descriptors.
6.	Specifying the data points for every cluster such that the items in the same cluster (as similar as possible), but the items that belong to the diverse clusters are as various as possible.
7.	Every center of the cluster key points, and their close neighbors are matched only to other clusters rather than assembling all the other key points. <br>

![image](https://github.com/LameUser/Copy-Move-Detector/assets/73399578/61076087-b01f-4957-9ab0-3ddbb8003b07)




## Working Principle

Image forgery means manipulation of the digital image to conceal some meaningful or useful information of the image. There are cases when it is difficult to identify the edited region from the original image. The detection of a forged image is driven by the need of authenticity and to maintain integrity of the image.
The most frequently used technique for image tampering is copy-move which aims to hide or manipulate the content of the image. This paper surveys the different approaches applied for detecting copy-move forgery.

The image forgery approaches are basically classified into two types namely active and passive approaches. Both approaches use different techniques, and they are classified further which is shown in Figure. 

![image](https://github.com/LameUser/Copy-Move-Detector/assets/73399578/a1640bf8-c38a-4ca0-b5c7-5f2db32e692c)



## Detection Results and Comparison

Here we are considering the most used techniques, copy-move and Splicing method, where we have done analysis on some images which we have forged using the copy-move method only.
There are many software’s and websites available to change the pixels, width, frames, depth detailing inside a picture. Every software makes changes inside the original picture which can be easily detected by the tampering done to it. There are many existing ways to check the authenticity of an image. We are using copy-move method for the detection, below are some examples of the result.



Output for an original image:

![image](https://github.com/LameUser/Copy-Move-Detector/assets/73399578/ac7dc627-1526-4332-93d9-59b3c9c91ed9)




Output for a forged image:

![image](https://github.com/LameUser/Copy-Move-Detector/assets/73399578/ca3bc7af-6beb-4354-8822-d2935c4bf7f7)



## Author

**_[LameUser](https://github.com/LameUser)_**
