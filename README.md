# Opening-and-Closing

## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step 1:
Import the necessary packages


### Step 2:
Create the Text using cv2.putText

### Step 3:
Create the structuring element

### Step 4:
Use Opening operation

### Step 5:
Use Closing Operation

### Step 6:
end the program.
 
## Program:

``` Python

DEVELOPED BY: HARSHAVARDHINI M
REG NUMBER: 212221240015

# Import the necessary packages

import numpy as np
import cv2
import matplotlib.pyplot as plt

# Create the Text using cv2.putText

img1=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX
im=cv2.putText(img1,' MONISHA T ',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(im)

# Create the structuring element

Kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(11,11))

# Use Opening operation

image1=cv2.morphologyEx(im,cv2.MORPH_OPEN,Kernel)
plt.imshow(image1)


# Use Closing Operation

image1=cv2.morphologyEx(im,cv2.MORPH_CLOSE,Kernel)
plt.imshow(image1)




```
## Output:

### Display the input Image
![download](https://user-images.githubusercontent.com/93427208/171139168-153ff968-9ca6-4b66-8fae-18047a045d82.png)

### Display the result of Opening

![download](https://user-images.githubusercontent.com/93427208/171139220-6f9f39b9-b585-4ef9-a3e1-92ab0dd81c70.png)

### Display the result of Closing
![download](https://user-images.githubusercontent.com/93427208/171139241-35f3eea0-5c5a-4609-a893-1a600bd81cd0.png)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
