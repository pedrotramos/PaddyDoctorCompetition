# Identifying the type of disease present in paddy leaf images

This repository is the result of my work in a Kaggle competition called **Paddy Doctor: Paddy Disease Classification**.

## The Problem:

Rice (Oryza sativa) is one of the staple foods worldwide. Paddy, the raw grain before removal of husk, is cultivated in tropical climates, mainly in Asian countries. Paddy cultivation requires consistent supervision because several diseases and pests might affect the paddy crops, leading to up to 70% yield loss. Expert supervision is usually necessary to mitigate these diseases and prevent crop loss. With the limited availability of crop protection experts, manual disease diagnosis is tedious and expensive. Thus, it is increasingly important to automate the disease identification process by leveraging computer vision-based techniques that achieved promising results in various domains.

## The Objective:

The main objective of this competition is to develop a machine or deep learning-based model to classify the given paddy leaf images accurately. Provided of a training dataset of 10,407 (75%) labeled images across ten classes (nine disease categories and normal leaf) and, also, additional metadata for each image, such as the paddy variety and age. Your task is to classify each paddy image in the given test dataset of 3,469 (25%) images into one of the nine disease categories or a normal leaf.

## The Solution:

The solution adopted was based on an article named [Deep Learning based Feature Extraction for Texture Classification](https://www.researchgate.net/publication/341906662_Deep_Learning_based_Feature_Extraction_for_Texture_Classification), which was written by **Philomina Simon** and **Uma Vijayasundaram**. The article suggests the usage of Deep Learning to extract features from the original images and further use of the extracted features as input for faster models like SVM or Random Forest. This approach results in a fast, yet effective model, which might be interesting for applications in regions with poor internet connectivity, such as many rural areas across the globe. I also implemented data augmentation (SMOTE) to ensure the training dataset was balanced.

## The Result:

The baseline for this project was the performance of the model developed by the creators of the competition. Their model achieved an accuracy score of 93.83%. Therefore, my objective was to beat this mark. Luckily, the outcome was quite positive and my model scored **97.35%** in terms of accuracy in the test set.

![My competition score](./assets/competition_score.png)



