# **Finding Lane Lines on the Road** 

## Goal

For all given images of the video we need to find and recognaze the lane lines on left and right sides.

---

## Algirithm

My algorithm consisted of 9 steps.

### *Step one*
Convert the image to HLS color space.

### *Step two*
Filtered a white and yellow lines.

### *Step three*
Convert the image to GrayScale color space.

### *Step four*
Gaussian blur on the image is helps us reduce noise.

### *Step five*
Canny edge detection. We used this algorithm to detect edges on the image. 

### *Step six*
Defining region of interest helps us concentrate our attention only current region, region where we find the lane lines. 

### *Step seven*
Apply Hough transform to detect lines on our image.

### *Step eight*
Separeting lines between left and right side by slope. First of all we must filter horizontal and vertical slope.

### *Step nine*
And finally, we add these lanes to our original image.

## Identify potential shortcomings with your current pipeline

First of all my lane lines are rattling.

Second potential shortcoming would be what would happen when we lost one of any lane lines, doesn't matter left or right one. 

And finally shortcoming could be if rain will happen. I think my algorithm will not abble to see the mirrored lane lines. 


## Suggest possible improvements to your pipeline

A possible improvement would be to apply linear reggression to find mean slope of lines.

Another potential improvement could be to new apgorithm to detect lane lines after rain too.
