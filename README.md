# Road Line Detection Project

## Overview
This project focuses on detecting **road lane lines** in video input using computer vision techniques. It aims to support applications like autonomous vehicles and driver assistance systems by identifying lane boundaries in real-time. The detection system processes each video frame, enhances the region of interest, and highlights the lane lines on the road.

## Dataset
This project uses a sample video file, typically a dashcam recording (`road_car_view.mp4`), which contains real-world road footage. The video demonstrates two-lane road scenarios and is processed frame-by-frame.

### Input Example:
- **road_car_view.mp4**: Sample driving video used for detection.

## Preprocessing Steps
To enhance lane detection, the following image processing steps were applied:
1. **Gaussian Blur**: Reduces noise and smoothens the image.
2. **Color Space Conversion**: Converts each frame to HSV for better color filtering.
3. **Color Thresholding**: Applies color mask to isolate yellow lane lines using HSV values.
4. **Canny Edge Detection**: Detects edges in the masked image.
5. **Hough Line Transformation**: Detects and draws lane lines on the original frame.

## Output
- **Live Video Window**: Displays real-time frame with detected lane lines.
- **Edge Window**: Displays the result of Canny edge detection.

## Additional Resources
You can use more road footage from various online datasets or dashcam videos to test the model further.

