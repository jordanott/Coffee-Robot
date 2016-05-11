# CoffeeRobot
RaspberryPi CV module that tracks the state of a coffee pot

## Prerequisites

- [Setup OpenCV 3 for Python](http://www.pyimagesearch.com/2015/02/23/install-opencv-and-python-on-your-raspberry-pi-2-and-b/)
- [Setup Numpy on Raspberry Pi](http://wyolum.com/numpyscipymatplotlib-on-raspberry-pi/)
- ...other things (setup email/notification service, camera, wifi, etc...)

## Description

- This project detects how full/empty a coffee pot is using opencv in python
- We first constructed haar cascades using ~500 positive coffee pot images and ~900 negatives
- The cascade files were used to locate the pot within the image
- Then within the space of the located pot we used line detection to find the line of the coffee
- Based off the found line relative to the rest of the pot we could accurately determine the level of coffee in the pot
