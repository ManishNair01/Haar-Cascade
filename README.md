# Iris Flower Recognition using Haar Cascade Algorithm

## Overview

This project employs a Haar Cascade algorithm for recognizing iris flowers in images. Unlike traditional machine learning models, Haar Cascade is an object detection algorithm that uses a trained cascade classifier for detecting objects in images or video frames. In this case, it will be adapted for iris detection.

## Dataset

For training and testing the Haar Cascade algorithm, a dataset containing images of iris flowers was used. The dataset includes positive samples with labeled iris regions and negative samples without iris regions.

## Haar Cascade Algorithm

The Haar Cascade algorithm is based on a machine learning approach, where a cascade function is trained from positive and negative samples. OpenCV provides tools for training cascade classifiers, allowing the creation of a classifier specifically tailored for iris detection.

## Training

The training process involves using positive and negative samples to train the cascade classifier. The trained classifier is then used to detect iris regions in new images.

```bash
# Example command for training Haar Cascade classifier using OpenCV
opencv_traincascade -data output -vec positive_samples.vec -bg negative_samples.txt -numStages 10 -minHitRate 0.999 -maxFalseAlarmRate 0.5 -numPos 1000 -numNeg 500 -w 20 -h 20
