# **Finding Lane Lines on the Road** 

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road

* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 6 steps. 

Step 1, I converted the images to grayscale.
Step 2, I made an gaussian smoothing,and chose the kerne_size as 5.
Step 3, I made canny detection,and the low_threshold and high_threshold are 50 and 150 seperatly.
Step 4, I kept the region of interest.
Step 5, I made Hough transform for line detecting
Step 6, I draw lines on a blank image.

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by
averaging the slop angle of each lane and calculate the start point of each lane in the picture. 

### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when the car is shift the lane

Another shortcoming could be wrong detection for lane.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to the canny detection part.

Another potential improvement could be to keep the region of interest.
