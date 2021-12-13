# Image Mosaicing

Image mosaicing is an effective means of constructing a single seamless image by aligning multiple partially overlapped images. 


### Algorithm for two images

1. Find the keypoints and descriptiors of two images using SIFT
2. Fnd the matches using FlannBasedMatcher and KNN
3. Extract good matches from them with a threshold (0.3 is used for this project)
4. Find the homography matrix for both the images using RANSAC
5. Transform one image to other using homography matrix
6. Stich the two images and remove black pixels if any

#### Results 

- Panorama of given images


### Algorithm for stiching multiple images

1. Given a set of images, calculate descriptors for all using SIFT
2. Apply above algotithm for every two images
3. Keep removing black pixels if any

#### Results

- Panorama of given images
