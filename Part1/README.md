# CMU Pose, Illumination, and Expression (PIE) Database

This repository contains the implementation and experimentation results for the CMU Pose, Illumination, and Expression (PIE) database. The PIE database consists of 41,368 images of 68 subjects, each captured under 13 different poses, 43 different illumination conditions, and with 4 different expressions [[1]](http://ieeexplore.ieee.org/abstract/document/1004130/).

For this project, we use a simplified version of the database, which includes 10 subjects and contains five near-frontal poses. The dataset consists of 170 images per individual, and all images have been resized to 32x32 pixels. The dataset is provided in the form of a CSV file with 1700 rows and 1024 columns. Each row represents an instance, and each column represents a feature. The first 170 instances belong to the first subject, the next 170 to the second subject, and so on. The following images illustrate various instances of the first subject.

## Project Overview

The main objective of this project is to preprocess the dataset, create random splits for training and testing, and evaluate the performance of a k Nearest Neighbors (k-NN) classifier. Additionally, we will incorporate the dimensionality reduction technique Principal Component Analysis (PCA) to observe its impact on computation times, classification performance, and the correlation of covariance matrices.

## Requirements

To replicate the experiments and evaluate the results, the following requirements must be met:

1. Preprocessing and Random Splits:
   - Normalize each face image vector to unit length by dividing each vector by its magnitude.
   - Randomly select 150 images from each subject for training and use the remaining 20 for testing.
   - Repeat the random splits a total of 5 times.
   - Report the average accuracy and standard deviation over the 5 random splits, along with computation times.

2. k Nearest Neighbors (k-NN) Classifier:
   - Implement a k-NN classifier using the training set.
   - Experiment with different distance measures, such as Euclidean, Mahalanobis, and cosine similarity.
   - Explore different values of k.
   - Present results with varying numbers of classes (subjects) involved in the experiments.
   - Include results when using fewer training images (e.g., 100 training images and 70 test images per category).

3. Dimensionality Reduction using PCA:
   - Apply PCA as an unsupervised technique to the training images.
   - Examine the effect of PCA on the correlation of covariance matrices by visualizing them before and after dimensionality reduction.
   - Analyze the impact of PCA on computation times and classification performance.
   - Vary the number of principal components used and identify the best number.

## References

[1] CMU Pose, Illumination, and Expression (PIE) Database. Available at: [http://ieeexplore.ieee.org/abstract/document/1004130/](http://ieeexplore.ieee.org/abstract/document/1004130/)

---

Note: The above README script provides an outline
