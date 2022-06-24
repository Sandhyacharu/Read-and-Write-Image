### EX NO: 01
### DATE:
# <p align="center">READ AND WRITE AN IMAGE</p>
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
```
### Developed By:N Sandhya Charu
### Register Number: 212220230041
```
i) #To Read,display the image
```python3
  import cv2
  color_image = cv2.imread("image.jpg",1)
  cv2.imshow('212220230041',color_image)
  cv2.waitKey(0)
  gray_image = cv2.imread("image.jpg",0)
  cv2.imshow('212220230041',gray_image)
  cv2.waitKey(0)
```
ii) #To write the image
```python3
cv2.imwrite("image1.jpg",gray_image)

```
iii) #Find the shape of the Image
```python3
  color_image.shape
  gray_image.shape
```
iv) #To access rows and columns
```python3
  import random
  for i in range (100):
      for j in range(color_image.shape[1]):
          color_image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]

```
v) #To cut and paste portion of image
```python3
  tag = color_image[200:320,200:320]
  color_image[280:400,280:400] = tag
  cv2.imshow('212220230041',color_image)
  cv2.waitKey(0)

```

## Output:

<br>

### i) Read and display the image

![image](https://user-images.githubusercontent.com/75235167/161373171-20a693d9-84af-43c6-ac2d-65f28106f051.png)

<br>

![image](https://user-images.githubusercontent.com/75235167/161373280-83324666-c349-41e0-b5a8-205dfbf615e9.png)

<br>

### ii)Write the image
<br>

![image](https://user-images.githubusercontent.com/75235167/161373272-6c270be7-83a7-4d38-aa38-803cc5838155.png)

<br>

### iii)Shape of the Image

<br>

![image](https://user-images.githubusercontent.com/75235167/161373294-a61dbcfa-e220-446f-b03c-9af4a59aeb25.png)

<br>

### iv)Access rows and columns

<br>

![image](https://user-images.githubusercontent.com/75235167/161373404-b65f8e1b-e863-40bc-a676-5194cd9788aa.png)

<br>

### v)Cut and paste portion of image

<br>

![image](https://user-images.githubusercontent.com/75235167/161373540-f2a22c99-216f-463b-a703-10584d245286.png)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.

