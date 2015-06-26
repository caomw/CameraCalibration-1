# CameraCalibration
This program determines the distortion and the camera matrix

## what it does
This program determines the distortion and the camera matrix using OpenCV. The output is an XML or YAML File telling you the camera instrinsic and distortion coefficients. 

## usage
    $ ./cameraCalibration
    
## requires
* cmake 2.8
* openCV
* gcc

## tested on
* Ubuntu 14.04
* gcc 4.8.2
* cmake 2.8.12.2
* openCV 2.4.8

## to do
* Implementation

## literature
* [OpenCV tutorial](http://docs.opencv.org/doc/tutorials/calib3d/camera_calibration/camera_calibration.html)

## example output
The output will be a loooong xml file. With a loooot of information. Most probably you need to know the Camera Matrix and the Distortion Coefficients.
The Camera Matrix is stored in the *Camera_Matrix* -child node *data* and the Distortion Coefficients are stored in the *Distortion_Coefficients* -child-node *data*. So far so easy. But what number stands for what.
*Camera_Matrix* consists of 9 elements in row and the elements stand for

1. **fx**
2. **0**
3. **cx**
4. **0**
5. **fy**
6. **cy**
7. **0**
8. **0**
9. **1**

*Distortion_Coefficients* consists of 5 elements in row and the elements stand for

1. **k1**
2. **k2**
3. **p1**
4. **p2**
5. **k3**
