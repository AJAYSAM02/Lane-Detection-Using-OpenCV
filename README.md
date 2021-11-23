# Lane-Detection-Using-OpenCV
Using CV(Computer Vision) techniques in Python identifying road lane lines.
Generally for self driving cars as the self-driving cars should not cross it’s lane and should not go in opposite lane to avoid accidents.

To detect white markings in the lane we need to mask the rest part of the frame. This is done using frame masking. The frame is a NumPy array of image pixel values.
After this we need to detect lines and for this purpose we will use Hough Transform. The Hough transform is a technique which can be used to isolate features of a particular shape within an image. Hough transformation can detect shapes like rectangles, circles, triangles, and lines.

Steps:
1. importing all the necessary libraries
2. apply frame masking
3. Hough transformation(conversion of pixels to a line)
4. create two lines in each frame
5. processing each frame to detect lanes
6. clip the input video file to frames and get the resultant output video.

Result: Using CV we were able to do lane detection. Before detecting lane lines, we masked remaining objects and then identified the line with Hough transformation.
