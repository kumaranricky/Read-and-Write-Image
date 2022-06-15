# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
```python
# Developed By:KUMARAN.B
# Register Number:212220230026
# To Read,display the image

import cv2
bw=cv2.imread("AM.jpeg",1)
cv2.imshow('212220230026-kumaran',bw)
cv2.waitKey(0)
#GREY IMAGE
gray=cv2.imread("AM.jpeg",0)
cv2.imshow("greyimage",gray)
cv2.waitKey(1)

# To write the image
cv2.imwrite("naturekumaran.jpeg",bw)

# Find the shape of the Image
print(bw.shape)

# To access rows and columns
import random
for i in range(100):
    for j in range(bw.shape[1]):
        bw[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('accessing row and column',bw)
cv2.waitKey(0)

# To cut and paste portion of image
bw2=cv2.imread("AM.jpeg",1)
tag=bw2[400:500,400:500]
bw2[50:150,50:150]=tag
cv2.imshow("cutting portion",bw2)
cv2.waitKey(0)


```
## Output:

### i) Read and display the image
![o1](https://user-images.githubusercontent.com/75243072/173726592-efe1e14a-aa72-4db5-8144-d712ffea9817.png)

### grey image
![o2](https://user-images.githubusercontent.com/75243072/173726618-c29a6dfe-d656-421c-abd9-338d7b26b020.png)

### ii)Write the image
![o6](https://user-images.githubusercontent.com/75243072/173726684-1a00ee6c-e788-46ed-8aed-f31597285010.png)

### iii)Shape of the Image
![o3](https://user-images.githubusercontent.com/75243072/173726659-5a7b7c2c-9474-4315-8fb9-faea9906e561.png)

### iv)Access rows and columns
![o4](https://user-images.githubusercontent.com/75243072/173726743-338a4e6e-f098-46d2-8fb0-703e30dd6bb7.png)

### v)Cut and paste portion of image
![o5](https://user-images.githubusercontent.com/75243072/173726772-38ab978e-a9b7-4b8a-8cb5-ff5d65ae839e.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


