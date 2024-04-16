# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages
### Step2:
Create the Text using cv2.putText
### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

## Program:
```
Developed by:Samyuktha S
Register Number:212222240089
```
### Display the input Image
```
import cv2
import numpy as np

img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'SAMYUKTHA', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)
```
### Create ths structured element
```
struct_ele = np.ones((9, 9), np.uint8)
```
### Display the result of Opening
```
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
### Display the result of Closing
```
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:

### Display the input Image
![image](https://github.com/SamyukthaSreenivasan/OPENING--AND-CLOSING/assets/119475703/31db3094-96ba-45be-a587-6bc895bd31b4)

### Display the result of Opening
![image](https://github.com/SamyukthaSreenivasan/OPENING--AND-CLOSING/assets/119475703/d0db1940-7c93-42bc-9d9e-d4c6fec34a86)

### Display the result of Closing
![Uploading image.png…]()


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
