# CarVisulisation 1.0
Uses a car visulasation system as described 

Homography transformations involve a mathematical mapping between two planes. When you have two images of the same flat surface, but taken from different perspectives or angles, a homography can be used to map points from one image to the corresponding points in the other image. In this project it would be used to map the detected vehicles and road features from a camera view to a coordinate system used in the simulation environment.

This transformation is described by a 3x3 matrix, and it operates on the homogeneous coordinates of the points (which means the coordinates are represented with an extra dimension, usually set to 1).
The transformation can be expressed as:

<p align="center">
  <img src="https://github.com/user-attachments/assets/f2421cd2-c8d0-4574-ab13-67a4e236a96e" alt="lagrida_latex_editor">
</p>


Here
* (x,y) are the coordinates in the original image (e.g., camera view).
* (x',y') are the coordinates in the transformed image (e.g., bird's-eye view).
* H is the 3x3 homography matrix that defines the transformation.

## This matrix 𝐻 can be computed if you know at least four corresponding points between the two views. Once H is determined, any point in the original image can be mapped to the new perspective.

## Example output!


https://github.com/user-attachments/assets/c8b7f442-993a-4ef7-9321-c1e8accd34c4






### How to use?
1. I recommend using colab
2. Download/clone the repo, download the YOLO('yolov8l.pt') file which is already in the notebook
3. Run with the files given

### What i plan to add
* Pedestrians
* Change of direction to be detected 
* Smoother motion, animations to be added.
* Give the option to choose a car model etc.
