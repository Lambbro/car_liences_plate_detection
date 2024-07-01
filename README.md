#This respository is about building a detection model of detecting car liences plate
##Using yolov8 model to detect car plate and easyocr to read that plate

First of all, dataset we used is from [Kaggle](https://www.kaggle.com/datasets)
This dataset is separated into test, train, validation files with images and their label

This is and example 
![image](https://github.com/Lambbro/car_liences_plate_detection/assets/100024864/26c031bd-a2f4-473f-88b3-5e53bc84fd1f)
'1', '0.28398895790200135', '0.6459627329192547', '0.4095928226363009', '0.6563146997929606', '0.3819875776397516', '0.722567287784679', '0.26328502415458943', '0.7111801242236024'
Its label is an array with first element is type of plate. Vietnamese Plate has 2 type is 1 line plate (0) and 2 line plate (1)
Others are 4 pairs of coordinates represent for 4 corner points of the plate
And this is the image with line drew of plate
![image](https://github.com/Lambbro/car_liences_plate_detection/assets/100024864/fd6d4916-0c00-49b6-838e-a276d23f5b79)

With label, we easily train yolo8 model to detect in other image
![image](https://github.com/Lambbro/car_liences_plate_detection/assets/100024864/5e5fc8ee-df2c-416f-a099-a42cbbad81cb)
The percentages are accuracy of corners to draw around of the plate

Combine with easyocr model, we can read those liences plates in every image
1 example of plate in above image
![image](https://github.com/Lambbro/car_liences_plate_detection/assets/100024864/d8eac55a-8505-4e63-b95e-e585fc77ff57)

Finally, We can read and show the plate or just show their hometown
![image](https://github.com/Lambbro/car_liences_plate_detection/assets/100024864/3e9bfe19-2ad7-45c5-9027-1e11683cf0ff)
