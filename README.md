# Crime Detection Using Surveillance Cameras

## Project Overview

This project aims to automatically detect different types of crimes from surveillance camera footage using deep learning and computer vision techniques.  
It can identify activities like assault, robbery, shoplifting, vandalism, and more by analyzing video frames extracted from security cameras.

## What This Project Does

- Extracts frames from videos of various crime scenes.
- Detects people and objects in these frames using a pre-trained model.
- Enhances the quality of these images to improve detection.
- Trains a neural network to classify different types of criminal activities based on the enhanced images.

## What You Will Find in This Repository

- **Code files** for extracting frames from videos.
- **Scripts** for detecting objects in frames using YOLOv5.
- **Image enhancement** code applying filters and contrast improvement.
- **Trained model** code to classify crime types.
- **Dataset folder structure** showing categories of crimes like Assault, Robbery, Shoplifting, etc.
- **Example output images** showing detected objects and enhanced frames.
- **Plots** of training and validation accuracy and loss for the model.

## How to Use

1. Put your video dataset in the folder with subfolders for each crime category.  
2. Run the frame extraction script to convert videos into images.  
3. Use the object detection script to find important objects in each frame.  
4. Enhance these images with the provided filters to improve clarity.  
5. Train the classification model using the enhanced images to recognize crime types.  
6. Check the output folders to see detected and enhanced images, as well as model training results.

## Dataset Structure

Dataset/
├── Abuse/
├── Arrest/
├── Arson/
├── Assault/
├── Burglary/
├── Explosion/
├── Fighting/
├── RoadAccidents/
├── Robbery/
├── Shooting/
├── Shoplifting/
├── Stealing/
└── Vandalism/


Each folder contains video clips related to that crime.

## Results

- The model achieves high accuracy in identifying different crimes.
- Training and validation plots are included to show model performance.
- Enhanced images help improve detection accuracy.

---

This system can help automate monitoring of surveillance footage to quickly identify potential crimes and alert authorities.

---

## Author

Sandhya Rani N 
November 2025

