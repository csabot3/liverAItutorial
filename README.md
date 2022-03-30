# Liver AI Tutorial
This is a tutorial for working with radiology data and AI models of the liver which is designed to be run via Google Colab.

## Lesson 1: Data Basics

Basics of working with DICOMs in Python.

## Lesson 2: Liver Segmentation

U-net segmentation of the liver on CT and MRI using the CHAOS dataset and FastAI. Divided into 2 parts to separately cover CT and MRI segmentation.

## Lesson 2, Part 1: Liver Segmentation on CT

U-net segmentation of the liver on CT data using FastAI and the CHAOS dataset.

## Lesson 2, Part 2: Liver Segmentation on MRI

U-net segmentation of the liver on MRI data using FastAI and the CHAOS dataset. Covers scenarios involving only segmenting the liver and scenarios with multi-organ segmentation.

## Lesson 3: Radiomics Basics

Exploration of utility of organ segmentations for further data analysis. We highlight the SimpleITK and Pyradiomics packages for further analysis of radiology segmentation data. 

## Lesson 4, Part 1: Neural Networks Revisited with CT Data

Lesson 4 revisits the neural network concepts of lesson 2 but places a greater emphasis on modeling details such as training data image augmentation, the learning rate, the loss function, the optimizer, and the neural network architecture. The first part of lesson 4 uses CHAOS CT data to investigate the impact of these varias aspects of neural network modeling on a simple classification neural network which is designed to classify whether or not an axial CT slice contains liver parenchyma. 

## Lesson 4, Part 2: Neural Networks Revisited with MRI Data

We conclude this series of lessons by revisiting the MRI data in CHAOS and showing some examples of how modeling can go wrong. We demonstrate an example of a flawed setup of training and validation datasets in which axial slice data from the same patient cases is intermixed between the training and validation dataset when patient studies have the same labels across every slice. We also explore alternative setups for working with FastAI by using Pandas dataframes. We conclude the lesson with an alternative setup to the U-net segmentation performed in lesson 2 with an emphasis on attention to pre-trained weights versus random weights and freezing subsets of weights during training.
