# Face Recognition using Haar Cascade Algorithm

## Overview

This project utilizes a Haar Cascade algorithm for face recognition in images or video streams. The Haar Cascade is an object detection algorithm that can be trained to detect faces in images. In this project, OpenCV is used for implementing the Haar Cascade face recognition.

## Dataset

For training and testing the Haar Cascade algorithm, a dataset containing images of faces was used. The dataset includes positive samples with labeled face regions and negative samples without face regions.

## Haar Cascade Algorithm

The Haar Cascade algorithm is a machine learning-based approach to object detection. It uses a trained cascade classifier to identify objects, such as faces, in images. OpenCV provides tools for training cascade classifiers, enabling the creation of a classifier specific to face detection.

## Training

The training process involves using positive and negative samples to train the cascade classifier. The trained classifier is then used to detect faces in new images.

```bash
# Example command for training Haar Cascade classifier for face detection using OpenCV
opencv_traincascade -data output -vec positive_samples.vec -bg negative_samples.txt -numStages 10 -minHitRate 0.999 -maxFalseAlarmRate 0.5 -numPos 1000 -numNeg 500 -w 20 -h 20
