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
### Developed By:
### Register Number: 
i) #To Read,display the image
```
  import cv2
  color_image = cv2.imread("image.jpg",1)
  cv2.imshow('212220230041',color_image)
  cv2.waitKey(0)
  gray_image = cv2.imread("image.jpg",0)
  cv2.imshow('212220230041',gray_image)
  cv2.waitKey(0)
```
ii) #To write the image
```
cv2.imwrite("image1.jpg",gray_image)

```
iii) #Find the shape of the Image
```
  color_image.shape
  gray_image.shape
```
iv) #To access rows and columns
```
  import random
  for i in range (100):
      for j in range(color_image.shape[1]):
          color_image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]

```
v) #To cut and paste portion of image
```
  tag = color_image[100:120,100:120]
  color_image[80:100,80:100] = tag
  cv2.imshow('212220230041',color_image)
  cv2.waitKey(0)

```

## Output:

### i) Read and display the image

<br>
<br>

### ii)Write the image

<br>
<br>

### iii)Shape of the Image

<br>
<br>

### iv)Access rows and columns
<br>
<br>

### v)Cut and paste portion of image
<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


