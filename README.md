# Internship Tasks Repository

This repository contains the tasks assigned for the internship at Cowlar Inc. The tasks focus on implementing and analyzing different algorithms and techniques in the field of computer vision and machine learning. The following are brief descriptions of the tasks:

## Task 1: CMU PIE Database Analysis
In this task, we explore the CMU Pose, Illumination, and Expression (PIE) database. The goal is to preprocess the dataset, perform random splits for training and testing, and evaluate the performance of a k Nearest Neighbors (k-NN) classifier. We experiment with different distance measures, values of k, and the number of classes involved. Additionally, we examine the impact of using different numbers of training images. The repository provides Jupyter Notebooks for each step of the analysis, along with the dataset and experimental results.

## Task 2: Lazy Snapping Image Cut-Out / Segmentation
The focus of this task is to implement the Lazy Snapping algorithm for interactive image cut-out and segmentation. The algorithm utilizes partial human annotations in the form of foreground and background "seed" pixels. The implementation involves performing K-Means clustering on color pixels, extracting seed pixels for each class, and calculating the likelihood of a given pixel belonging to the foreground or background. Finally, pixels are assigned to the class with the higher likelihood. The repository includes the implementation code, test images, and comparisons of results obtained with different values of clusters.
