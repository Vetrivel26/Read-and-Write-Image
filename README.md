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
### Developed By:Vetri Vel S
### Register Number: 212221240060
### i)To Read,display the image
```
import cv2
color_image=cv2.imread('acd.jpeg',1)
cv2.imshow('colorimage',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
### ii)To write the image
```
cv2.imwrite('adc.jpeg',color_image)
cv2.imshow('academia Image',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()



```
### iii)Find the shape of the Image
```
import cv2
color_image=cv2.imread('acd.jpeg',-1)
print(color_image.shape)



```
### iv)To access rows and columns

```
import cv2
import random
color_img=cv2.imread('acd.jpeg',1)
for i in range(150):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
        cv2.imshow('212220230042, P.Sanjay',color_img)
cv2.waitKey(0)
cv2.destroyAllWindows()



```
### v)To cut and paste portion of image
```
cut=color_image[260:280,100:300]
color_image[60:80,100:300]=cut
cv2.imshow('cutimage',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()



```

## Output:

### i) Read and display the image

![img1](https://user-images.githubusercontent.com/75235426/161391662-46337ed8-2fdc-4edf-92d5-393fec774c41.png)


### ii)Write the image

![img2](https://user-images.githubusercontent.com/75235426/161391693-bf2344a2-d21f-49a9-89b7-ac272bbb49bc.png)

### iii)Shape of the Image

![img3](https://user-images.githubusercontent.com/75235426/161391707-e1c076d4-e26f-4d5e-9fbd-5cda54376d1b.png)

### iv)Access rows and columns
![img4](https://user-images.githubusercontent.com/75235426/161391718-464621a9-9461-4898-87ee-a0267c57584e.png)

### v)Cut and paste portion of image
![img5](https://user-images.githubusercontent.com/75235426/161391732-d9b03443-5c84-44e0-8002-2c2a5080bc85.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


