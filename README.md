# Deep-Learning-Model-for-Artistic-Style-Transfer
This project demonstrates the application of neural style transfer using the VGG16 model. It involves taking two images, a content image and a style image, and blending them together so the output image looks like the content image but painted in the style of the style image.


Dataset Link : https://drive.google.com/drive/folders/12E-BDjAbKRFRwWV0wXyUYMN7P2mg7qa7?usp=drive_link

Requirements
Python 3.x
PyTorch
TorchVision
PIL (Python Imaging Library)
Matplotlib
NumPy
Requests
Installation
Install Python: Ensure that you have Python 3.x installed on your system. You can download it from python.org.

Install Required Libraries:
import torch
import torch.optim as optim
from torchvision import models, transforms
from PIL import Image
import matplotlib.pyplot as plt
import numpy as np
import requests

Usage
Prepare Images: Place the content and style images in a known directory.

Set Image Paths: In the main script, set the content_path and style_path variables to the paths of your content and style images, respectively.

Run the Script: Execute the cells one by one.

Code
Dashtoon_Shruti
View Results: The final styled image will be displayed alongside the original content image.

Components
ImageLoader: Handles loading and processing of images.

VGG16FeatureExtractor: Wraps around the VGG16 model to extract features from the images.

StyleTransfer: Performs the neural style transfer by optimizing the content and style representations.

Main Execution Block: Initializes the process, executes the style transfer, and displays the results.

Notes
Ensure your machine has compatible hardware (GPU) for faster processing, although the script can run on a CPU as well.
Adjust the steps parameter in the StyleTransfer class for more or fewer iterations during style transfer.
The script can be modified to support different models or additional functionalities as needed.
