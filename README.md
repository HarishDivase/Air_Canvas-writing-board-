# Air_Canvas-writing-board-
Using OpenCV to identify and map hand motions onto a PiTFT screen, Air Canvas is a hands-free digital art canvas.
OpenCV was used to construct a computer vision project.
Ever longed to use a finger in the air to sketch anything in your head? In this article, we'll discover how to create an Air Canvas that can be used to create any image by just using a camera to record the movement of a coloured marker. Here, the marker is a coloured item held at the tip of the finger.

To develop this project, we'll be utilising OpenCV's computer vision methods. The preferred language is python because of its extensive libraries and simple syntax, but by grasping the fundamentals, it can be implemented in any language that supports OpenCV.
Here, the goal is accomplished by using colour detection and tracking. A mask is created once the colour marker is identified. It also comprises the subsequent morphological processes of erosion and dilation on the finished mask. Erosion removes the impurities from the mask, and dilatation further repairs the primary mask that has been eroded.
# Algorithm
1. Begin reading the collected frames and convert them to HSV colour space. (Easy to discern colours)
2. Set the appropriate ink buttons on the canvas frame and prepare the canvas.
3. Modify the trackbar values to locate the coloured marker mask.
4. Apply morphological procedures on the mask as a preprocess.
Erosion and enlargement
5. Identify the contours, locate the greatest contour's centre coordinates, and maintain saving them in the array for subsequent frames.
Drawing points on a canvas with arrays
6. At last, draw the array's points on the frames and canvas.

You must have python3, numpy, and opencv installed on your computer.
