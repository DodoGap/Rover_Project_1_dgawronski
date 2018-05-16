## Project: Search and Sample Return
---



* I added the same functions to Jupyter Notebook, and file `perception.py` named `find_rocks` which is similar to function `color_thershold`, because is choosing out the rocks color and returning 'black and white' image with selected rock. If function `find_rocks` is returning any data, map is filled with square which is position of finded rock.
* I modified function `process_image()` to transform images into view from isometric perspective, I add color threshold with masked view of camera to overcome unnecessary pixels, which is defined in `perspect_transform`. `perception.py` is also reading current position of rover and mapping it to world map, what is seen as red and blue marks on map

[//]: # (Image References)

[image1]: ./misc/rover_image.jpg
[image2]: ./calibration_images/example_grid1.jpg
[image3]: ./calibration_images/example_rock1.jpg 
[image4]: ./output/warped_example.jpg 
[image5]: ./output/mask_example.jpg

## [Rubric](https://review.udacity.com/#!/rubrics/916/view) Points

---

### Notebook Analysis
#### 1. I added a few lines to `perspect_transform()`, at first I added mask (white triangle as u can see on image below) to output warped images, be sure, there won't be any unnecessary pixels or stuff.

![alt text][image4]



#### 1. Populate the `process_image()` function with the appropriate analysis steps to map pixels identifying navigable terrain, obstacles and rock samples into a worldmap.  Run `process_image()` on your test data using the `moviepy` functions provided to create video output of your result. 
And another! 

![alt text][image2]
### Autonomous Navigation and Mapping

#### 1. Fill in the `perception_step()` (at the bottom of the `perception.py` script) and `decision_step()` (in `decision.py`) functions in the autonomous mapping scripts and an explanation is provided in the writeup of how and why these functions were modified as they were.


#### 2. Launching in autonomous mode your rover can navigate and map autonomously.  Explain your results and how you might improve them in your writeup.  

**Note: running the simulator with different choices of resolution and graphics quality may produce different results, particularly on different machines!  Make a note of your simulator settings (resolution and graphics quality set on launch) and frames per second (FPS output to terminal by `drive_rover.py`) in your writeup when you submit the project so your reviewer can reproduce your results.**

Here I'll talk about the approach I took, what techniques I used, what worked and why, where the pipeline might fail and how I might improve it if I were going to pursue this project further.  



![alt text][image3]


