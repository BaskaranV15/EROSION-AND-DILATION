## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
mport the necessary libraries (OpenCV and NumPy).
### Step2:
Use cv2.putText to add the text "BASKARAN.V" to the img1 image at specific coordinates.


### Step3:
Define two kernels (kernel and kernel1) for morphological operations.
### Step4:
Display the eroded image using cv2.imshow.
### Step5:
 Use cv2.waitKey(0) to wait for a key press indefinitely.


## Program:

``` Python
# Import the necessary packages
import cv2
import numpy as np
# Create the Text using cv2.putText
img1=np.zeros((100,400),dtype="uint8")
font=cv2.FONT_HERSHEY_PLAIN
cv2.putText(img1,"BASKARAN.V",(5,70),font,2,(255),5,cv2.LINE_AA)
cv2.imshow("image",img1)
cv2.waitKey(0)



# Create the structuring element
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))



# Erode the image

image_erodel1=cv2.erode(imag1,kernel1)
cv2.imshow("baskaran212222230020",image_erodel1)
cv2.waitKey(0)
cv2.destroyAllwindows()

# Dilate the image


image_dilate1=cv2.dilate(imag1,kernel1)
cv2.imshow("baskaran21230020",image_dilate1)
cv2.waitKey(0)


```
## Output:

### Display the input Image

![Screenshot from 2023-10-10 18-35-01](https://github.com/BaskaranV15/EROSION-AND-DILATION/assets/118703522/be1cb15b-a64d-482d-a983-aacb580ec38b)


### Display the Eroded Image

![Screenshot from 2023-10-10 18-36-16](https://github.com/BaskaranV15/EROSION-AND-DILATION/assets/118703522/978c97b7-ee78-4d45-b7de-100cee030af1)


### Display the Dilated Image


![Screenshot from 2023-10-10 18-37-29](https://github.com/BaskaranV15/EROSION-AND-DILATION/assets/118703522/61cdeeea-da62-4f79-a6a6-f764fe478497)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
