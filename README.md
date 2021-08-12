<!-- PROJECT LOGO -->
<br />
<p align="center">
  <h3 align="center">Hand Detection</h3>

  <p align="center">
    Hand segmentation using Skin color and Motion Detection
    <br />
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

Human-Computer Interaction using hand gesture recognition is a great advancement in technology that makes our life easier and convenient. For any gesture recognition, Hand detection is important that is a pre-processing step. In this project, hand segmentation is done using skin color and motion detection using thresholding. Using a web camera, the hand is segmented and then we can use it in any application. 

### Built With

* [Python](https://www.python.org/)
* [Opencv](https://opencv.org/)

<!-- GETTING STARTED -->
## Getting Started

This is how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Hardware

A simple web cam or any other external camera. For the programing 


### Installation

List of things you need to install.
* pip

  ```sh
  pip install opencv-python 
  ```
  ```sh
  pip install imutils
  ```
  ```sh
  pip install numpy
  ```
## Libraries

Opencv - Opencv is a library for computer vision, machine learning and image processing.


### Apply threshold value to the image

Befor applying it, need to convert image into grayscale
```sh
thresh = cv.threshold(imgray, 127, 255, 0)
```
### Draw contours

```sh
contours, hierarchy = cv.findContours(thresh, cv.RETR_TREE, cv.CHAIN_APPROX_SIMPLE)
```

<!-- USAGE EXAMPLES -->
## Usage

Hand gesture recognition use in many areas for human-computer interaction. For robot control, virtual environments, television controls, etc. For any geture recongnition system, accurate hand detection is necessary. Accurate hand detection can give more accurate outcome in applications. 

## Results

#### Hand Detection using Skin color

#### Hue, Saturation and Value color model

![HSV](https://user-images.githubusercontent.com/77574279/129238612-b716ac3b-d889-46cd-8473-36d1e5a389ca.jpg)

#### YCbCr (Luminance and Chrominance color model)
![YCbCr_](https://user-images.githubusercontent.com/77574279/129238674-44d13cb4-9dcc-4287-a3bb-aff4585116b7.jpg)

#### Result - Combination of HSV and YCbCr color model
![Final](https://user-images.githubusercontent.com/77574279/129238720-0c24c948-7b43-4e14-82d4-b8fb3443ab95.jpg)


### Hand detection using motion detection using thresholding

![Contours](https://user-images.githubusercontent.com/77574279/129239666-12739d4e-39ed-4248-ae4e-4f47e6adf326.jpeg)

![Thresholded](https://user-images.githubusercontent.com/77574279/129239707-2bb68369-107f-453f-8bf6-f6e0680c19c9.jpeg)



<!-- CONTACT -->
## Contact

Your Name - Hemang Parmar - hparmar6@lakeheadu.ca.com

Project Link: [https://github.com/HemangParmar/Hand-Detection](https://github.com/HemangParmar/Hand-Detection)


## References

https://docs.opencv.org/4.5.2/d6/d00/tutorial_py_root.html

[https://github.com/CHEREF-Mehdi/SkinDetection]

[https://github.com/dtaneja123/Hand_Recognition/blob/master/Hand_gesture_final.py]




