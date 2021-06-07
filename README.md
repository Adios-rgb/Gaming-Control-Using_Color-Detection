# Gaming-Control-Using_Color-Detection
Contour detection using HSV masking for lateral gaming movement.

# Functionality

* Uses masking to create contours, detects and tracks the contour.
* The contour is tracked for left and right movement which is simulated in the game.

![game_demo_gif](https://user-images.githubusercontent.com/59373491/121060822-c19fa900-c7e0-11eb-8560-96ed3d5fb944.gif)

# Packages used

* OpenCV
* Numpy
* imutils
* pydirectinput
* time
* win32api

# Steps Involved

* Turn on the webcam which will act as input source.
* Create a mask to track particular colour.
* Apply image processing such as dilate, opening, closing to reduce noise.
* Find contours on the processed image, get the maximum contour.
* Apply logic to remove reverse effect of the webcam (left-right, right-left).
* Press left button if the object you are tracking exceedes maximum left threshold and same logic for right movement.
* Display the frame.
