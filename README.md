# Edge-Linking-using-Hough-Transform
## AIM:
To write a Python program to detect the lines using Hough Transform.

## SOFTWARE REQUIRED:
Anaconda - Python 3.7

## ALGORITHM:
### Step1:

Import all the necessary modules for the program.
### Step2:

Load a image using imread() from cv2 module.
### Step3:

Convert the image to grayscale.
### Step4:

Using Canny operator from cv2,detect the edges of the image.
### Step5:

Using the HoughLinesP(),detect line co-ordinates for every points in the images.Using For loop,draw the lines on the found co-ordinates.Display the image.


## PROGRAM:

```
DEVELOPED BY : HIBA NASREEN M
REG NO : 212224040117
```
### Input image and grayscale image
```python
import numpy as np
import cv2
import matplotlib.pyplot as plt

gray = cv2.imread('nature.jpg', cv2.IMREAD_GRAYSCALE)
img_color = cv2.imread('nature.jpg', cv2.IMREAD_COLOR)
img_c = cv2.cvtColor(img_color, cv2.COLOR_BGR2RGB)
gray_rgb = cv2.cvtColor(gray, cv2.COLOR_GRAY2RGB)

gray = cv2.GaussianBlur(gray, (3, 3), 0)
```
```python
plt.figure(figsize=(13, 13))
plt.subplot(1, 2, 1)
plt.imshow(img_c)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1, 2, 2)
plt.imshow(gray_rgb, cmap='gray')
plt.title("Gray Image")
plt.axis("off")
plt.show()
```

### Canny Edge detector output
```python
import numpy as np
import cv2
import matplotlib.pyplot as plt

gray = cv2.imread('nature.jpg', cv2.IMREAD_GRAYSCALE)
img_color = cv2.imread('nature.jpg', cv2.IMREAD_COLOR)
img_c = cv2.cvtColor(img_color, cv2.COLOR_BGR2RGB)
gray_rgb = cv2.cvtColor(gray, cv2.COLOR_GRAY2RGB)

gray = cv2.GaussianBlur(gray, (3, 3), 0)
```
```python
plt.figure(figsize=(13, 13))
plt.subplot(1, 2, 1)
plt.imshow(img_c)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1, 2, 2)
plt.imshow(gray_rgb, cmap='gray')
plt.title("Gray Image")
plt.axis("off")
plt.show()
```

### Display the result of Hough transform
```python
import numpy as np
import cv2
import matplotlib.pyplot as plt
```
```python
gray = cv2.imread('nature.jpg', cv2.IMREAD_GRAYSCALE)
img_color = cv2.imread('nature.jpg', cv2.IMREAD_COLOR)
img_c = cv2.cvtColor(img_color, cv2.COLOR_BGR2RGB)
gray_rgb = cv2.cvtColor(gray, cv2.COLOR_GRAY2RGB)

gray = cv2.GaussianBlur(gray, (3, 3), 0)
```
```python
plt.figure(figsize=(13, 13))
plt.subplot(1, 2, 1)
plt.imshow(img_c)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1, 2, 2)
plt.imshow(gray_rgb, cmap='gray')
plt.title("Gray Image")
plt.axis("off")
plt.show()
```

## OUTPUT:

### Input image and grayscale image

<img width="991" height="833" alt="image" src="https://github.com/user-attachments/assets/e2d7c722-b145-449c-8127-c26db0a6afae" />


### Canny Edge detector output

<img width="283" height="508" alt="image" src="https://github.com/user-attachments/assets/2078663e-df93-406d-9ca4-6ea52989f66a" />


### Display the result of Hough transform

<img width="283" height="514" alt="image" src="https://github.com/user-attachments/assets/7e3dd5ab-583a-4dcb-8f40-75bf18442088" />


## RESULT:

Thus, the image has been successfully converted.

