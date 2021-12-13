# OPENCV-Plate-Number-Detector
Program that detects and stores images of Russian car plate numbers, using OpenCV, Haarcascades and Python

This software uses OpenCV library to detect Russian car plate numbers using camera. 

Program is written in plateDetector.py file. 

Default camera is your laptop's webcam, set in the instruction "cap = cv2.VideoCapture(0)", 0 stands for default webcam. 

You may change the camera setting to another camera. To do so, please read the OpenCV documentation. 

# Project structure 
The project consists of plateDetector.py file where entire logic for the plate detection is placed and Resources folder.

Resources folder consists of a single haarcascade_russian_plate_number.xml file, which is used to detect the Russian car plate numbers, and two folders: Images and Scanned 

Images folder contains three testing images of cars bearing Russian plates, we will use those to test our software. 

Scanned folder is currently empty. Once we run the program we will be able to scan the plate numbers and store those images here in Scanned folder.

# How to use 

run the plateDetector.py file 

Your webcam will turn ON 

I have provided 3 testing images of cars with Russian plate numbers. Personally, I've uploaded those images on my smartphone and simply pointed the screen of my smartphone towards te webcam, to allow the software to see the test image and recognize the plate number. However, feel free to use the testing images as you see fit to test out this program. 

The plateDetector will detect the plate numbers and highlight them with a purple square around them and text "Number Plate" next to the square. 

The second window will open containing only plate number that is visible. 

Press "s" to scan the plate number. You will see a large writting "SCAN SAVED" across the screen. The program will take the screenshot of the plate number only (as seen in the second window containing only the number plate) and save the image in Scanned subfolder of Resources folder. Images will be marked with a serial number and stored in .jpg format. 

Press "q" to close all windows. 

