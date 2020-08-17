# AR-App

This Augmented Reality application was built by me for TCS to showcase contactless shopping experience for customers.

It has been built using Untiy 3D engine + Vuforia SDK.

Unity enables you to build an android app and it integrates with Vuforia SDK which does the heavy lifting with Image and 3D Object recognition capabilities for the app. You can read more about it here: https://library.vuforia.com/getting-started/overview.html

All the apps mentioned below can be downloaded from this drive link: https://drive.google.com/drive/folders/1c0Ox4Ag_rkQGjc_RjZRiEJDhMQ9dEHMR?usp=sharing

------------------------
Image recogniser
------------------------
For images, we need to train the model by uploading the image to Vuforia developer portal. It will extract relevant features (like SIFT) and train a binary classifier to detect the image. The trained model can be downloaded onto the system and packaged along with the unity app for offline detection.

Steps:
1. The model was trained to recognise the image  in "Road1.tex.jpg" and overlay it with a 3D object (easily available in Unity store).
2. Download and install the ARImgDemo.apk file. Open the app. Click on "Let's Start".
3. Open the image "Road1.tex.jpg" and scan it using the app. You should be able to see a tiny 3D car overlaid on the image if the detection is successful.

------------------------
3D Object recogniser
------------------------
For 3D objects, we need to scan the model 360deg on a marker reference provided by Vuforia so that the scale and 3D model is accurately captured. The SDK also provides the quality of scan and lets you know if it needs to be rescanned. Rest of the process is very similar to image recognition.

For detection of a 3D object through the ARObjDemo.apk file (another app), you need to have a pre-scanned 3D object with you which is not possible :(. So won't be able to showcase this.
