# **Finding Lane Lines on the Road** 

---

**Finding Lane Lines on the Road**

The goals of this project:
* Understand the process to develop and run an algorithm to identify lane marks on the Road

The steps that I took to achieve the goal are the following:
* First step is select the files to work with
* Apply filters to improve the recognition of the lane edges and mark the edges
* Tweek the parameters in snapshots do make more acurate result
* Finnaly apply the optimal result on the video and correct any abnormal artifects that may appear



[//]: # (Image References)

[image1]: ./examples/line-segments-example.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consists of 5 steps. First, I converted the images to grayscale, then I applied filters of blur to reduce the amount of noise present in the image, in doing so the key elements of the image more recognizable. Third applied the Canny transform to high light the most proeminent edges. Forth I chose the region of intesrest, the lane marks are ina predictable plase, so we don't need to look at the intire image and finnaly we can use apply the annotation on the images ans videos.


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when we have shadows cast on the road or lane changes. the algorithm might not work propperlay in may inpredictable cases that may occur in not ideal conditions;

Another shortcoming could be that the video annotation is very unstable and this might lead to errors in a real world scenario.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to use the sobel to detect edges.
