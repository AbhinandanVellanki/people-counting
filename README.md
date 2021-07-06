# People counting system 

## Short Overview
The system counts the people entering and leaving an entrance, using a Deep Neural Network as a detector (YOLOv3) and a tracking algorithm to track and count (DCF-CSR \ CSRT). It was developed by myself and Or Farfara as a project in Machine Learning & Computer Vision at the Technion, and intended for use by the Technion's libraries (though it could be optimized for any entrance).

## Setup
- Clone repo
- Install dependencies in requirements.txt file 
- Download the detector YOLOv3-416's .weights file from here: https://pjreddie.com/darknet/yolo/
- Convert the .weights file into .h5 and insert it into the model_data folder.

## Important notes and how to use
- You *should* read the user's manual attached https://github.com/IdoGalil/People-counting-system/blob/master/Counting%20System%20User's%20manual.pdf
- The system has some parameters that should be optimized to the specific entrance it's used on. Most importantly, DI and MCDF.
- For more information about the components and ideas of the system and how they were developed, read the project's report.
- The code is relatively modular, in such a way it would be easy to modify the detector and the tracker components as better updated ones are made.
- The system is intended for real-time performance (more info in the report), and as such requires GPU. note that it could recieve its input from an IP camera, but to work in near real-time the video must be obtained at high speeds.

#### This repository is a modification of 
https://github.com/IdoGalil/People-counting-system

