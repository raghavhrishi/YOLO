# PyTorch Implementation of YOLO:
Original Paper: https://arxiv.org/abs/1506.02640


Object detection is a fundamental task in computer vision. The problem of object recognition essentially consists of first localizing the object and then classifying it with a semantic label. In recent deep learning based methods, YOLO is an extremely fast real time multi object detection algorithm.
## Data Pre-Processing 
The current format of the labels are (class, x1, y1, x2, y2), where x1, y1 are the top left corner of the bounding box and x2, y2 are the bottom right corner of the bounding box.

## Required Features:
* Image shape -> 128x128x3
* The Image is split into 8x8 patches with each representing a 16x16 grid.
* Each grid is responsible for detecting the object whose center falls into the grid.
* For each anchor, there are 8 channels, which encode Pr(Objectness), x, y, w, h, P(class=pedestrian), P(class=traffic light), and P(class=car).
