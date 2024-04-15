# imageAnalysis

 changeDetection - 

This program is designed to detect significant changes in a video stream and trigger an alarm accordingly. The primary functionality revolves around real-time image processing to monitor deviations from a predefined background state.

Steps:

1.Camera Connection: Initiate a connection to the camera.

2.Background Setup: Capture an initial background image, convert it to grayscale, and store it as a floating-point image for further analysis.

3.Detection Loop:
  Image Acquisition: Continuously acquire new images from the camera.
  Preprocessing: Convert each new image to grayscale and then to floating-point format.
  Change Detection: Compute the absolute difference between the new image and the background image.
  Apply a threshold to this difference image to create a binary image that highlights areas of significant change.
  Alarm Decision: If the percentage of foreground pixels exceeds a predefined alert threshold (A), trigger an alarm and display a message on the image.
