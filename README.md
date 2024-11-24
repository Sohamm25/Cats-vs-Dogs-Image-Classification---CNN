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
## How to Run the Notebook
Clone this repository and navigate to the project folder.
Install the required packages:
bash
Copy code
pip install -r requirements.txt
Run the Jupyter Notebook to view and execute the code:
bash
Copy code
jupyter notebook Dogs_vs_Cats_Image_Classification_CNN.ipynb
