## Libraries Used
I'm planning on using C++ with raspicam and OpenCV to achieve basic facial detection. I would like the program to notify our phones when a face is recognized by the door, but this may only be feasible for me in Python.

#### Raspicam
https://github.com/cedricve/raspicam

#### Picamera2 - (Python)
https://datasheets.raspberrypi.com/camera/picamera2-manual.pdf

#### Raspi camera software docs
https://www.raspberrypi.com/documentation/computers/camera_software.html

#### Debug command line
Start server on PI - libcamera-vid -t 0 --inline --listen -o tcp://0.0.0.0:8069
Connect to that server - ffplay tcp://192.168.0.125:8069 -vf "setpts=N/30" -fflags nobuffer -flags low_delay -framedrop
