# computer-vision-in-arduino
This repository contains information about implanting convolutional neural network in arduino mega 2560

Machine Learning Model that I'm dealing with is trained using "Machine Learning Tool"
check for this link: https://github.com/Hanheum/Machine_Learning_Tool_4

sd card directories tree:

-imgs
 -(images in specific form*)
-nn
 -(machine learning model save files*)
 
*specific form of image:
  1) load image in PIL
  2) convert to numpy array
  3) normalize array by dividing array by 255.0
  4) round at 6 digits below 1 to save as numbers as float (float in arduino is 4 bytes, but python is 8 bytes)
  5) use struct to convert floats to byte array
  6) save bytes in one file

*machine learning model save files:
  After you train your model in machine learning tool, make sure enable arduino option in model class. And also use save_for_arduino function to save.
  
For more information, contact here:
chh3653@gmail.com
