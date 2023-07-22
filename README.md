# Depth Estimation Using Stereo Matching
## Introduction:
- Depth estimation is a critical task for autonomous driving. It’s necessary to estimate the distance to cars, pedestrians, bicycles, animals, and obstacles.
The popular way to estimate depth is LiDAR. However, the hardware price is high, LiDAR is sensitive to rain and snow, so there is a cheaper alternative: depth estimation with a stereo camera. This method is also called stereo matching.
## The main idea:
- In general, the idea behind the stereo matching is pretty straightforward.
- We have two cameras with collinear optical axes, which have a horizontal displacement only. We can find a corresponding pixel on the right camera frame for every pixel on the left camera frame. We can estimate the point’s depth if we know the distance between pixels related to this point on the left and right frames. As one can see from the depth of the point is inversely proportional to the distance between the images of this point. This distance is called a disparity:
- ![stereo](https://learnopencv.com/wp-content/uploads/2020/09/disparity.png)
## ![stereomatching](https://drive.google.com/uc?export=view&id=1E6yGt6xllneuxnR2sMlaIG2AH7g0wEYV) 
## Pipeline
- ![pipeline](https://drive.google.com/uc?export=view&id=1Tt9TrDmILezdV69C_vB9H-yiW5b_xRtZ)
- In range of this project, I just research Stereo matching computation using 3 method:
  + Pixel-wise matching method.
  + Window-based matching method.
  + Cosine Similarity (based on the window-based matching disparity map)
## References:
- AI Viet Nam
- https://learnopencv.com/depth-estimation-using-stereo-matching/
