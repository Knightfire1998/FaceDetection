# FaceDetection
#### In this project a simple face detector has been created using Haar Cascade Method.

# What is Haar Cascade ?
Haar Cascade is a machine learning object detection algorithm used to identify objects in an image or video and 
based on the concept of features proposed by Paul Viola and Michael Jones in their paper "Rapid Object Detection using a Boosted Cascade of Simple Features" in 2001

# What are Haar Features ?
Haar features are sequence of rescaled square shape functions proposed by Alfred Haar in 1909. They are similar to convolution kernels 
taught in the Convolution Neural Networks course. We will apply these haar features to all relevant parts of face so as to detect human face.  

![Haar Feature](https://github.com/Knightfire1998/FaceDetection/blob/master/haar.png?raw=true)  
As we see in the above image, there are edge features (1 and 2), line features (3).  
They are white and black pixels images (value 0 or value 1).  
But usually we have greyscale/colour image (pixel value range from 0 to 255).  

# Working : -
1. We use a opencv and haar feature file (it contains feature description for face and eyes of a person) as a base for our face detector.
2. Video feed is captured using the webcome with the help of **cap.read()** method in openCV, then it is converted into frames.
3. Then the Frames are processed one at a time, a Cascadeclassifier with Haar feature file as an input tries to match all the features of the frame with the features in the file.
4. Bounding boxes are drawn around the detected face and eyes.

![Face Detection](https://github.com/Knightfire1998/FaceDetection/blob/master/face.jpg?raw=true)  

# Requirements :-
#### 1. Python 3.*  
#### 2. OpenCV  
#### 3. Numpy  

# Links for reading : -
![Haar like Features](https://en.wikipedia.org/wiki/Haar-like_feature)  
![Cascade Classifier](https://docs.opencv.org/3.4/db/d28/tutorial_cascade_classifier.html)  
![Face Detection using Haar like Features](https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_objdetect/py_face_detection/py_face_detection.html)
