#Facedetect batch processesing example

This example has been worked from the haar detector originally bundled with 
the opencv 2.1 documentation. Its been hacked to act as a batch slurper. It is given a directory and goes through and systematically tags/moves
all the images it thinks have faces in them.

>This program is demonstration for face and object detection using haar-like features.
>The program finds faces in a camera image or video stream and displays a red box around them.
>Original C implementation by:  ?
>Original Python implementation by: Roman Stanchak, James Bowman

##Usage:
python facedetect.py some/directory 

This program will go through all the images found under `some/directory` and look for any that 
contain faces. If it finds one, it'll create a copy with face_ prepended to the file name.
any interesting features will be highlighted by a red rectangle

##Detecting other things:
I have enclosed sample haar aml definitions that were bundled with opencv. They have a 3 clause BSD license which can be seen here:
[Here](http://opencv.org/license.html) to use them in this programme simple change the cv.load() function to use an XML file of your
choice. (line 54) The enclosed definitions are well labeled.


