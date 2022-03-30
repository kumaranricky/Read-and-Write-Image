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
![o1](https://user-images.githubusercontent.com/75243072/160784720-1cda2d08-b3bc-49e6-b3d4-88eb363b9ffd.png)
### grey image
![o2](https://user-images.githubusercontent.com/75243072/160784732-3e0fc9eb-3091-4072-a97d-6af3b01c42c4.png)

### ii)Write the image

![o6](https://user-images.githubusercontent.com/75243072/160786128-413d06cb-c310-4631-a5ee-5cb16c4061f0.png)



### iii)Shape of the Image


![o3](https://user-images.githubusercontent.com/75243072/160786053-f4706e0e-06ed-4f67-bbe4-9bb1fefcd677.png)




### iv)Access rows and columns

![o4](https://user-images.githubusercontent.com/75243072/160784742-4e188c1f-5f56-45d2-8ae1-a9d082b3f949.png)

### v)Cut and paste portion of image

![o5](https://user-images.githubusercontent.com/75243072/160785016-6fe8092e-33ce-4846-8697-eda5bf34173e.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


