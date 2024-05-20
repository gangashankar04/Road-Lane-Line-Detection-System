# Road-Lane-Line-Detection-System

Road Lane Detection requires to detection of the path of self-driving cars and avoiding the risk of entering other lanes. Lane recognition algorithms reliably identify the location and borders of the lanes by analyzing the visual input. 

# Assumptions

1.Driving on the right side of a two-lane road (see the image for an example)

![rllds](https://github.com/gangashankar04/Road-Lane-Line-Detection-System/assets/170317051/fdcefb16-c75e-4449-8b0c-ba6348f4996e)


2.Driving during daylight; due to limitations on a sufficient quality video, night time conditions were not tested.

# Algorithms

 1.Image Acquistion: Cameras are mounted on the vehicle, typically on the windshield near the rearview mirror,to capture the forward
                     imageview of the road.
                     
 2.Preprocessing: Grayscale Conversion- Convert the captured color images to grayscale to simplify processing as lane markings
                  Gaussian Blur- Apply this one to grayscale image to reduce noise and smoothen the image.
                    
 3.Edge Detection: Use the canny edge detection algorithm to detect edges in the image.

 4.Region Of Interest Selection: Define a region of interest in the image where lane lines are expected to be a trapezoidal area 
                               in the lower half of the image.

 5.Lane Line Identification: Filter out line segments based on their slope and position to identify the left and right lane lines.

 6.Lane Markings and Estimations:
                     To model the curvature and ensure smooth lane lines and improve stability.
                     

