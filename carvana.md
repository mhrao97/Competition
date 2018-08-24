Carvana Image Masking Challenge
-------------------------

What is Carvana?

As with any big purchase, full information and transparency are key. While most everyone describes buying a used car as frustrating, it’s just as annoying to sell one, especially online. Shoppers want to know everything about the car but they must rely on often blurry pictures and little information, keeping used car sales a largely inefficient, local industry.

Carvana, a successful online used car startup, has seen opportunity to build long term trust with consumers and streamline the online buying process.

An interesting part of their innovation is a custom rotating photo studio that automatically captures and processes 16 standard images of each vehicle in their inventory. While Carvana takes high quality photos, bright reflections and cars with similar colors as the background cause automation errors, which requires a skilled photo editor to change.

The challenge is to develop an algorithm that automatically remove the photo studio background. This will allow Carvana to superimpose cars on a variety of backgrounds. The task is analyzing a dataset of photos, covering different vehicles with a wide variety of year, make, and model combinations.

Dataset
-------------------------

The data can be found from Kaggle. 
	https://www.kaggle.com/c/carvana-image-masking-challenge/data

This dataset contains a large number of car images (as .jpg files). Each car has exactly 16 images, each one taken at different angles. Each car has a unique id and images are named according to id_01.jpg, id_02.jpg ... id_16.jpg. In addition to the images, some basic metadata is provided about the car like make, model, year and trim.

The task is to automatically segment the cars in the images in the test set folder.


Methods
----------
	1. Use of Pandas and Numpy
Pandas library provides easy to use data structures and data analysis tools in Python. NumPy library provides scientific computing in Python.

	2. Use of Keras
Keras is a powerful deep learning library for Tensorflow, CNTK and Theano. It provides a high-level neural networks API to develop and evaluate deep learning models. It is easy to use.
Keras models are trained on Numpy arrays of input data and labels.

Merits of Keras:
	a. Keras allows easy and fast prototyping.
	b. It supports both CNN and RNN and also combination of CNN and RNN
	c. Runs seamlessly on CPU and GPU.

	3. CNN
Convolutional Neural Networks or CNN is a feed forward artificial neural network. The connectivity pattern between the neurons were inspired by biological process - the connectivity pattern resembles the organization of animal visual cortex. CNNs have wide application for image recognition and classification problems.
CNN architecture is stacked by distince layers that transform input volume to an output volume. Some of the layers are listed below
	1. Convolution layer
	2. Pooling layer
	3. Loss layer

I have used ReLU activation in the hidden layers and sigmoid activation for the output layer.

