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
### Developed By: Lubindher S
### Register Number: 212222240056
i) #To Read,display the image
```
  import cv2
img = cv2.imread('abc.jpg', 0)
resized_img = cv2.resize(img, None, fx=0.8, fy=0.8)
cv2.imshow('212222240056', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
ii) #To write the image
```

import cv2
img=cv2.imread('abc.jpg',0)
cv2.imwrite('writed_walt.png',img)

```
iii) #Find the shape of the Image
```python3

import cv2
img=cv2.imread('abc.jpg',0)
print(img.shape)

```
iv) #To access rows and columns

```python3

import cv2
img = cv2.imread('abc.jpg', 0)
resized_img = cv2.resize(img, None, fx=0.8, fy=0.8)
for i in range(100, 250):
    for j in range(10, 50):
        resized_img[i][j] = 255  
cv2.imshow('212222240056', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
v) #To cut and paste portion of image
```python3

import cv2
img = cv2.imread('abc.jpg', 1)
tag = img[300:400, 300:400]
img[50:150, 50:150] = tag
cv2.imshow('212222240056', img)
cv2.waitKey(0)


```

## Output:
### i) Read and display the image
![Screenshot 2023-11-06 194440](https://github.com/lubindher/READ-AND-WRITE-IMAGE/assets/119559904/e0c5938c-df54-4e09-a216-327532844bce)


### ii)Write the image
![Screenshot 2023-11-06 195057](https://github.com/lubindher/READ-AND-WRITE-IMAGE/assets/119559904/e762bc17-743e-4c93-8ba8-3f1f446042d4)


### iii)Shape of the Image

![Screenshot 2023-11-06 195057](https://github.com/lubindher/READ-AND-WRITE-IMAGE/assets/119559904/a043c169-984f-4382-a7c1-203b7fb555c7)


### iv)Access rows and columns
![Screenshot 2023-11-06 195756](https://github.com/lubindher/READ-AND-WRITE-IMAGE/assets/119559904/c45b1be3-5701-4415-bc61-7cd3452050dd)


### v)Cut and paste portion of image
![Screenshot 2023-11-06 195945](https://github.com/lubindher/READ-AND-WRITE-IMAGE/assets/119559904/5d1b10e0-5422-4d03-870e-fbfae7a81e8f)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
