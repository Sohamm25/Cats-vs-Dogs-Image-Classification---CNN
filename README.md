# Dogs vs Cats Image Classification using CNN

## Overview
This project involves classifying images of dogs and cats using a Convolutional Neural Network (CNN). I aimed to build a robust image classification model by exploring multiple layers, hyperparameter tuning, and experimenting with various preprocessing techniques.

The journey of this project required significant effort, from understanding the dataset's characteristics to training and validating the model. I’ve also addressed challenges along the way, which were instrumental in refining my understanding of deep learning concepts.

---

## Features
- **Custom CNN Architecture**: I designed a CNN architecture tailored for this task, balancing accuracy and computational efficiency.
- **Preprocessing Pipeline**: Images were resized, normalized, and augmented to improve the model's generalization ability.
- **Experiments and Optimization**: Multiple experiments were conducted to optimize hyperparameters such as learning rate, batch size, and network depth.

---
## How to Run
- To run this project locally, follow these steps:

## Clone the Repository
First, clone the repository to your local machine:


git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Install Dependencies
Install the required Python libraries using pip from the requirements.txt file:


pip install -r requirements.txt
## Download the Dataset
Download the Dogs vs Cats dataset from Kaggle or any other source and place it in the appropriate folder (data/ or as mentioned in the notebook).

## Run the Jupyter Notebook
Launch Jupyter Notebook to open the notebook file:

jupyter notebook Dogs_vs_Cats_Image_Classification_CNN.ipynb
Execute the Code
Inside the notebook, run the cells sequentially to preprocess the images, define and train the model, and evaluate the performance.

## Key Challenges
One of the most challenging aspects was implementing the data augmentation pipeline. Managing overfitting and improving the model's performance required the use of techniques like:

```python
datagen = ImageDataGenerator(
    rescale=1./255,
    rotation_range=20,
    width_shift_range=0.2,
    height_shift_range=0.2,
    shear_range=0.15,
    zoom_range=0.15,
    horizontal_flip=True,
    fill_mode='nearest'
)
