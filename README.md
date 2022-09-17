# Creating-fake-thermal-images-using-Python

Unfortunately thermographic cameras are quite expensive and complicated to handle so I thought of a way to create fake thermal images from a normal webcam feed.

At the chair we are using Python and OpenCV to test the image processing algorithms. Using a webcam is also really easy in Python so lets begin from this basic example:


This is the result of this first approach.


<img src="https://github.com/noorkhokhar99/Creating-fake-thermal-images-using-Python/blob/main/Screen%20Shot%201444-02-20%20at%208.53.25%20PM.png">







This all depends heavily on the lightning conditions in the room. My face, hair, t-shirt and the door mostly consists of darker colors (so less intensity in the grayscale image). Since my body is usually warmer than the room I want the darker colors to be mapped to the higher temperatures. Fortunately the matplotlip colormaps also come with a inverted mode (just append _r to the end of the colormaps name). Also try changing the parameters vmin and vmax to get a more dynamic colormap.


https://matplotlib.org/2.0.2/examples/color/colormaps_reference.html
