# RetinoHealth

## Introduction

A serious eye condition associated with diabetes is diabetic retinopathy (DR). A five-level severity scale can be applied based on international protocol. But in order to optimise a grading model for strong generalizability, a substantial amount of balanced training data must be gathered, and this is particularly challenging for the high severity levels. Standard data augmentation techniques, such as random flipping and rotation, are unable to produce data with a significant degree of diversity. Retino Health is an application built to recognize Diabetic Retinopathy in patient's fundus images. Retino Health aims at helping patients with diabetes recognize their retinal problems sooner and get medical help faster. We will be using the GAN algorithm for training the model which will be detecting diabetic retinopathy in patients.

## GAN model
Generative Adversarial Network is what it stands for. It is applied to machine learning jobs requiring unsupervised learning. It consists of two models that recognise and analyze patterns in data input automatically. The two models are termed as **Generator** and **Discriminator**. They compete with one another to analyse, record, and replicate the differences present in a dataset. New instances that could have been produced using the original dataset can be produced using GANs.

## Model Performance
We have used the [**FGADR dataset**](https://csyizhou.github.io/FGADR/) to use as reference for the Discriminator to train on and classify the images generated by the Generator model. The discriminator is able to succcessfully classify the pictures with a grading accuracy of an **average of 80 percent**.

## Running the project

1. Download the prerequisite packages
    - Run the command ```pip install -r requirements.txt``` on your terminal.

2. Run the driver program
    - Run the ```run.bat``` file.       
    **OR**
    - Run the command ```python Main.py``` in your project's root directory

3. Upload dataset
    - Upload the Fundus dataset.
    - This will be used to generate images by the GAN model

4. Load GAN model
    - Click on Load GAN model to generate images

5. Load Diabetic Retinopathy Prediction model
    - Now load the Diabetic Retinopathy Prediction model by clicking on the button
    - This is a CNN model traned to classify the pictures into one of the five categories of Diabetic Retinopathy categories available in the dataset.

6. Make predictions on GAN images
    - Now make predictions on the severity category of the  images produced by the GAN model using the CNN model. 
    - Perform this by clicking on Generate GAN Image & Predict Severity.