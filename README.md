# Object-tracking-based-on-colour
Used for survilaance ,vehicle navigation 
Install pyautogui...
We use HSV colour format ,as lots of colour are easily identifiable by Humans as compared to RGB colour format which is less identifiable. 
Doing the colour calibaration of the object which we need to detect by adjusting the lower and higher values of Hue Saturation Value.
Read frames from the camera ..... Do the image pre processing like .. resizing the image ,  converting BGR image to gray scale then to Gaussian blur,passing the image throught the hsv colour format and determinig the object,,,
Perform erode and dilation (to remove noise from the image ,there will be sunlight ,object will have white dots to remove that )...
finding countours and drawing minimum enclosing circle ,find center of the countor area ,and drawing circle and center and determinig direction of the object based on radius ....
If radius of the circle bounding object is geeting bigger means getting close to the screen so print STOP and if radius small means far away print "FRONT" if object moving left Print "LEFT "
if moving Right ptint "RIGHT"
