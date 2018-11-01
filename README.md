# Face, Eyes, Smiling Mouth Detection from the Video Stream
It is the basic project in computer vision for detecting the Face,Eyes, Smiling Face using haar cascades features.

# STEP-1:

We have to create the cascade classes classifier or the objects using the CascadeClassifier method of CV2 library which takes the haar cascade (xml) files of Haar Like features as input to detect the features from the images.

Below is the link of the haar cascades files:
https://github.com/opencv/opencv/tree/master/data/haarcascades

# STEP-2:

Detect function takes two arguments are gray scale and colored image which is captured from the video stream and return the colored images with the rectangles detecting to the face, eyes and smiling mouth. Using detectMultiScale method of the haar cascades upper left corner, width, height of the rectangle can be find.

# INCREASE THE EFFICIENCY:

If we are not finding the efficient result then we will change the parameters to detectMultiScale method.We will increase the number of neighbors and scaling parameter.

# STEP-3:

Video Capture is the method of the cv2 library which is used to capture the video from the the webcam.For capturing the frames from the video we need to follow the below steps:

1- we make the object of the video capture class.

2- Call the read method of video capture class which returns the frame from the video stream.

3- Find the gray scale copy using cvtColor method of CV2 library.

4- Passing the gray and colored images to the detect function.

5- Creating the window for displaying the video with Face detection.

