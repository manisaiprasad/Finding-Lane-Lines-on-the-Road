# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. My pipeline.

My pipeline consisted of 6 steps. First, I converted the images to grayscale, 
then I Defined a kernel size and apply Gaussian smoothing on the image,
then I Defined parameters for Canny and applied  on the image,
Next i created a masked edges image,
then Defined the Hough transform and parameters
then we have drawn the lines which we got from the hough transform on original image
 
In order to draw a single line on the left and right lanes, I modified the draw_lines() helper function by my own function which will
append the left lines into a left single line as well right lines into a single right line then it will draw to the image

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


### 2.potential shortcomings with current pipeline


One potential shortcoming would be what would happen when many curves in the road 

Another shortcoming could be when lines are refelective  


### 3. Suggest possible improvements to pipeline

A possible improvement would be to converting it into hsv

Another potential improvement could be to setting up the lower and upper bound for color selecting
