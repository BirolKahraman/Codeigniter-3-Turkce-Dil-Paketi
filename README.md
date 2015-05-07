Python Extension for Accessing Video Devices
============================================

Some tricks using opencv and python tkinter interface. 
A very little parts of code may be copied from other public sources, I don't remember from where.

VideoCapture is a Python extension for Win32 which makes it possible to access video-capture devices (TV-Card, USB, AV GRABBER, Webcam). It consists of a low-level native module (vidcap.pyd) and a high-level module written in Python (pyvidcap.py) which should be used solely.

## example
```python
from pyvidcap import Device
stream = Device()
stream.saveSnapshot('image.jpg')
```
is PYQT
```python
from pyvidcap import Device
stream = Device()
buffer, width, height = self.getBuffer()
qimg = QtGui.QImage.fromData(buffer)
pixmap = QtGui.QPixmap.fromImage(qimg)
```
 

## requirements

python 3x
pillow module
vidcap module


