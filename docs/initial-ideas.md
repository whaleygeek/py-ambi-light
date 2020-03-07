How this might work
-------------------

1) Use a raspberry Pi camera as the sensor, with a PiZeroW and the camera case
(it is super tiny!)

https://thepihut.com/products/adafruit-raspberry-pi-zero-w-camera-pack-includes-pi-zero

2) Use this program as the basis to capture a still image
(we can capture them quite fast)

https://projects.raspberrypi.org/en/projects/getting-started-with-picamera/5

3) There looks to be some data saying we can capture quite fast 40-80fps
depending on how you do it

https://raspberrypi.stackexchange.com/questions/22040/take-images-in-a-short-time-using-the-raspberry-pi-camera-module

4) Use PIL/Pillow (Python imaging library) to process the image file
and extract the pixels from the capture
(an image is basically a 2D array of pixels with colour intensities, P
ython knows how to index into 2D arrays)

https://en.wikipedia.org/wiki/Python_Imaging_Library

5) Apply the averaging with a bit of Python code (Python is good at maths)

6) Drive the pattern out on to the NeoPixels
(use something like this library, which seems to be maintained still)

https://github.com/rpi-ws281x/rpi-ws281x-python/

7) The PiZeroW has wifi built in, so would be possible to remotely configure
from a laptop, for example, and you would then not need a HDMI screen at all.

8) Power it from a USB battery for a portable setup, or a USB wall plug for a
fixed installation.

9) Probably add a button to 'safe shutdown' the system, using gpiozero

https://gpiozero.readthedocs.io/en/stable/api_input.html#button

https://raspi.tv/2012/how-to-safely-shutdown-or-reboot-your-raspberry-pi

