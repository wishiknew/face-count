# face-count

This app detects the faces in a jpeg, png or gif file and outputs the number of faces present.

## How it works?
  * First I load the image using OpenCV.
  * For the gif files I use giflib since OpenCV doesn't support loading of Gifs.
  * Now after loading the image, I can start analyzing for faces.
  * Using the OpenCV library's Haar Cascade algorithm, I detect faces in an image.
  * An HAAR Cascade is an effective object-detection method proposed by Paul Viola and Michael Jones.
  * It is a machine learning based approach where a cascade function is trained from a lot of positive and negative images. It is then used to detect         objects in other images.
  
## Uses:
* [opencv](https://opencv.org/) - for jpeg and png images
* [giflib](http://giflib.sourceforge.net/)
* [jsoncpp](https://github.com/open-source-parsers/jsoncpp)

##  Platform
I am using a Windows machine with cygwin installed. 

## Build
 ``` make ```
## Run
The executable needs a image file as parameter.
 ``` .\FaceDetector.exe .\<your-image-file>```
 You will find a json file with image file's name in the folder.
 It will contain the number of faces in the image.
 
 MIT @[wishiknew](github.com/wishiknew)
