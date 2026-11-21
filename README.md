# -WORKSHOP-3-Canny-Edge-Detection
##  NAME : JANANI D
## REG NO : 212225040142

## Aim
To implement edge detection in an image using the Canny Edge Detection technique in OpenCV.

## Software Required
Anaconda - Python 3.7
OpenCV
NumPy
Matplotlib
Algorithm
## Step 1
Import the required libraries, OpenCV (cv2) and Matplotlib (pyplot).

## Step 2
Read the input image (filename.jpg) using the cv2.imread() function in grayscale mode.

## Step 3
Apply Gaussian Blur to the image using cv2.GaussianBlur() to reduce noise and smooth the image.

## Step 4
Apply the Canny Edge Detection technique using cv2.Canny() with threshold values 50 and 150 to detect edges.

## Step 5
Create a figure using Matplotlib to display the results.

## Step 6
Display the original grayscale image in the first subplot.

## Step 7
Display the detected edges in the second subplot.

## step 8
Use plt.show() to display both images.

## PROGRAM

import cv2
import matplotlib.pyplot as plt

img = cv2.imread('jan.jpg',cv2.IMREAD_GRAYSCALE)

blurred =cv2.GaussianBlur(img, (5,5),0)

edges = cv2.Canny(blurred, 50, 150) 

plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()


## OUTPUT:

<img width="782" height="482" alt="image" src="https://github.com/user-attachments/assets/8038e16f-457b-46dd-908e-92d7a35388c7" />


