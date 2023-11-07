# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages
### Step2:
Read the image
### Step3:
Create the structuring element or kernal element
### Step4:
Use Opening operation
### Step5:
Use Closing Operation
 
## Program:

``` Python
Import the necessary packages

import cv2
import numpy as np

Create the Text using cv2.putText
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_HERSHEY_PLAIN
cv2.putText(img1,'THEBOSS',(5,35),font,2,(255),5,cv2.LINE_AA)
cv2.imshow("SARGURU_212222230134",img1)
cv2.waitKey()
cv2.destroyAllwindows()

# Create the structuring element
kernal=np.ones((5,5),np.uint8)


# Use Opening operation
mg1o=cv2.morphologyEx(img1,cv2.MORPH_OPEN,kernal)
cv2.imshow("SARGURU_212222230134",img1o)
cv2.waitKey(0)
cv2.destroyAllwindows()


# Use Closing Operation
imglc=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernal)

cv2.imshow("SARGURU_212222230134",imglc)
cv2.waitKey(0)
cv2.destroyAllwindows()


```
## Output:

### Display the input Image


![Screenshot 2023-11-07 133059](https://github.com/Sargurukumaresan/OPENING--CLOSING/assets/119559840/35e55e4f-3089-4816-b778-06ccd5ae0605)


### Display the result of Opening

![Screenshot 2023-11-07 133141](https://github.com/Sargurukumaresan/OPENING--CLOSING/assets/119559840/1a3c7b66-ad05-4453-877d-26874381b438)



### Display the result of Closing


![Screenshot 2023-11-07 133204](https://github.com/Sargurukumaresan/OPENING--CLOSING/assets/119559840/a601c237-3a23-4ab3-b576-b4736df07dc6)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
