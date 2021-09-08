# Frequency detection from videos

Computer Vision Course Final Project

The task in this project is calculating fundamental frequency of structures. Knowing the frequency is important for calculating the stiffness and the material properties (such as elastic modulus) according to known equations – it can replace lab measurements. Also, according to the frequency we can estimate the load capacity that specific structure can hold, making sure the structure is not under resonance risk etc. In this project we will show a process done on a printed headphones stand printed in 3d printer from abs, but can be done on any different structure based on the same principals.

In this project different approaches were tested in order to calculate the funda- mental frequency of structures under vibration:
1. Tracking - recording the position of key point in each frame over time and calculate the number of maximum points. The fundamental frequency is the number of maximum points divided by the duration of the video (of course we dealt with edge cases).
2. One pixel intensity - recording the intensity of a pixel in each frame, the chosen pixel should be located as close as possible to the edge of the structure when it is balanced so low amplitudes will also be captured. The fundamental frequency is calculated as before.
3. Intensity of window - recording the sum of intensities in a specific window for each frame. This approach is giving more information than the One pixel intensity. The fundamental frequency is calculated as before.
4. Distance from camera - recording the sum of intensities in specific window from video taken from side view of the model. This methods is based on the distance of an object from the camera (as the distance grows the object becomes smaller). The fundamental frequency is calculated as before.
5. Optical Flow - counting how many times the model motion changes direc- tion. The fundamental frequency is calculated as before.
