# Traffic-Lights-Detector-Project
## Objective :
This system detects the traffic lights with TensorFlow object detection API, and then uses image 
processing techniques to classify the state of the traffic lights. If the traffic lights are “RED” or 
“YELLOW”, then it will show command “STOP” and if the traffic lights are”RED”, then it will 
show the command “GO”.

## 1. Abstract :
The goal of this project is to detect signal light boards in the various backgrounds through color 
segmentation and cascade filtering methods,extract and identify signal indication areas based on 
their relative position, luminance, and shape information execute signal indication status 
recognition based on color uniqueness.
We are building a python project of traffic light detector using Tensorflow object detection API 
that can approximately detect the colour of traffic light of image image using OpenCV and 
tensorflow .
In this Python Project, we will approximately identify the colour of traffic light from the image. 
The predicted colour may be one of ‘Red’ ,’Green’, ‘Yellow’ and then we will output the 
command as “Go” or “Stop”.
* Detect traffic light
* Classify into Red,Yellow/Green
* Output commands be like stop/go

## 2. Terminologies Used :
### 2.1 Tensor Flow :
TensorFlow provides a collection of workflows with intuitive, high-level APIs
for both beginners and experts to create machine learning models in
numerous languages. Developers have the option to deploy models on a
number of platforms such as on servers, in the cloud, on mobile and edge
devices, in browsers, and on many other JavaScript platforms. This enables
developers to go from model building and training to deployment much more
easily.
### 2.2 OpenCV :
OpenCV is short for Open Source Computer Vision. Intuitively by the name, it 
is an open-source Computer Vision and Machine Learning library. This library 
is capable of processing real-time image and video while also boasting 
analytical capabilities. It supports the Deep Learning frameworks, Tensor 
flow, Caffe, and PyTorch.
### 2.3 NumPy :
NumPy which stands for Numerical Python, is a library consisting of
multidimensional array objects and a collection of routines for processing
those arrays. Using NumPy, mathematical and logical operations on arrays can
be performed. NumPy is a Python package. It stands for ‘Numerical Python’. It is a library
consisting of multidimensional array objects and a collection of routines for
processing of array.

## 3. Prerequisites :
Additional python libraries required for this project are as below :
* TensorFlow (tf ) 
* OpenCV (cv2) 
Other packages we’ll be needing come as part of the standard Python library.

## 4. Contents of the Project :
* frozen_inference_graph.pb
* mscoco_label_map.pbtxt
* Test images to give input for the project
* For signal detection, we have a .pb file- this is a protobuf file (protocol buffer); 
It is a path to frozen detection graph. This is the actual model that is used for 
the object detection.
* The file with the .pbtxt extension holds it in text format. These are 
TensorFlow files. It contains list of the strings that is used to add correct label 
for each box.

## 5. Steps for the Traffic Signal Light Detection Project :
* First we have to import the required python libraries .
* After inputting the image it is sent to read that image and the image will 
be processed.
* Download data and unzip it to make availability of some deploy pbtxts 
in it.
* For object detection, initialize protocol buffer and model.
* Let’s make a call to the detect_traffic_lights() function with the 
PATH_TO_TEST_IMAGES_DIR, MODEL_NAME, Num_images parameters. 
* This function detects the colour of the traffic light and results the 
commands as if the color is red or yellow returns stop and false else if it 
is a green returns go and true.
* At last the input image is read, sends to the detect traffic lights function 
and display it.

## 6. Project File Structure :
* Importing required python libraries
* Code for detecting the color
* Loading Image into NumPy array
* Reading Images
* Plotting origin for Image
* Detecting traffic lights
* Function to read , detect , and output the result.

## Conclusion: 
This project presents a new method for identifying and recognizing traffic 
signal status in urban environments. Through combining the color, brightness, 
shape, and position characteristics of traffic signal light boards, light boards 
are accurately located in the sequential images. In the HSV color space, the 
color of traffic lights is determined by analyzing the pixel distribution of the H
component.
For future works, efforts are desirable to further improve the recognition 
accuracy of the current study. For example, we found excessive exposure or 
lack of exposure is likely to result in missed detection. More research is 
needed to identify the key issues associated with excessive or less exposure 
and improve detection accuracy. When large vehicles pass through an 
intersection and they may block the view of traffic lights
