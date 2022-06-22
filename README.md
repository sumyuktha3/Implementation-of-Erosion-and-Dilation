# IMPLEMENTATION OF EROSION AND DILATION
## AIM:
To implement Erosion and Dilation using Python and OpenCV.
## SOFTWARE REQUIRED:
1. Anaconda - Python 3.7
2. OpenCV
## ALGORITHM:
### Step 1:
Import the necessary packages.
### Step 2:
Create the Text using cv2.putText
### Step 3:
Create the structuring element.
### Step 4:
Erode the image.
### Step 5:
Dilate the image.

## PROGRAM:
### Developed by   : S.Sumyuktha Rani
### Register Number: 212220230050

```
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img1,'SUMMU',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img1)
plt.show()

# Create the structuring element
kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(9,9))

# Erode the image
image_erode1=cv2.erode(img1,kernel)
plt.axis('off')
plt.imshow(image_erode1)
plt.show()

# Dilate the image
image_dilate1=cv2.dilate(img1,kernel)
plt.axis('off')
plt.imshow(image_dilate1)
plt.show()
```

## Output:

### Display the input Image

![WhatsApp Image 2022-05-21 at 1 54 54 AM](https://user-images.githubusercontent.com/75235818/169698265-3a4068bb-5914-4c75-84ab-d02dbdf8208d.jpeg)

### Display the Eroded Image

![WhatsApp Image 2022-05-21 at 1 54 54 AM (1)](https://user-images.githubusercontent.com/75235818/169698230-04cfcfdd-37e1-4c7b-9e5d-27a8089d6ec1.jpeg)

### Display the Dilated Image

![WhatsApp Image 2022-05-21 at 1 54 54 AM (2)](https://user-images.githubusercontent.com/75235818/169698251-b781bb5a-e870-4d77-a112-60194afe577f.jpeg)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
