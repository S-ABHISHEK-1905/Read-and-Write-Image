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
### Developed By: S.ABHISHEK
### Register Number: 212221230002
i) #To Read,display the image
```
import cv2 as cv
capture=cv.imread("C:/Users/abhid/Downloads/a.jpg")
cv.imshow('PIC',capture)
cv.waitKey(0)
```

ii) #To write the image
```
import cv2 as cv
capture=cv.imread("C:/Users/abhid/Downloads/a.jpg")
cv.imwrite("photo.jpg",capture)
cv.imshow("PIC",capture)
cv.waitKey(0)
```

iii) #Find the shape of the Image
```
import random
import cv2 as cv
capture=cv.imread("C:/Users/abhid/Downloads/a.jpg")
print(capture.shape)
```

iv) #To access rows and columns
```
import random
import cv2 as cv
capture=cv.imread("C:/Users/abhid/Downloads/a.jpg")
for i in range(70,90):
    for j in range(110,170):
        capture[i][j]=[0,0,0]
cv.imshow("PIC",capture)
cv.waitKey(0)
```

v) #To cut and paste portion of image
```
import random
import cv2 as cv
capture=cv.imread("C:/Users/abhid/Downloads/a.jpg")
tag=capture[100:120,110:120]
capture[0:20,10:20]=tag
cv.imshow("PIC",capture)
cv.waitKey(0)
```

## Output:

### i) Read and display the image

<br>
![image](https://user-images.githubusercontent.com/66360846/224539236-950a4269-3bb0-4ebd-824d-1fa3a04c6cab.png)
<br>

### ii)Write the image

<br>
![image](https://user-images.githubusercontent.com/66360846/224539236-950a4269-3bb0-4ebd-824d-1fa3a04c6cab.png)
<br>

### iii)Shape of the Image

<br>
![image](https://user-images.githubusercontent.com/66360846/224539878-fada1a93-87f2-4830-b6fa-5f3b6b97c847.png)
<br>

### iv)Access rows and columns

<br>
![image](https://user-images.githubusercontent.com/66360846/224540052-aa89aafa-6b08-452f-a416-d0c01911e328.png)
<br>

### v)Cut and paste portion of image

<br>
![image](https://user-images.githubusercontent.com/66360846/224544688-2c51c381-a009-4c53-9295-4d5608cd0717.png)
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


