# CodeClauseInternship_FaceDetection

### Face detection using artificial intelligence (AI) involves the use of machine learning algorithms, specifically deep learning Convolutional Neural Networks (CNNs), to identify and locate human faces in images or videos. It is a significant step in facial recognition and has various applications in fields like security, biometrics, entertainment, and social media.

![image](https://github.com/pavankalyanchittala/CodeClauseInternship_FaceDetection/assets/117903644/d7b8f224-c5db-4426-9b6a-14936bb71fbf)



#### The implementation of face detection using OpenCV, a popular computer vision library in Python:Let's break down the code to understand its functioning:

-> The code imports the OpenCV library, which provides the necessary tools and functions for image processing and computer vision tasks.

-> The face_cascade object loads a pre-trained Haar cascade classifier, specifically the "haarcascade_frontalface_default.xml" file. This file contains the trained model for face detection.

-> The code initializes a VideoCapture object cap to access the webcam and captures video frames.

-> Inside the infinite while loop, the code reads each frame from the webcam using cap.read().

-> The image is then converted to grayscale using cv2.cvtColor() function. This step is necessary because the Haar cascade classifier works on grayscale images.

-> Face detection is performed using the detectMultiScale() function, which takes the grayscale image, a scale factor, and the minimum number of neighbor rectangles required for a detection. This function returns a list of rectangles representing the detected faces.

-> The code loops over each detected face and draws a rectangle around it using cv2.rectangle() function. It takes the image, the coordinates of the top-left and bottom-right corners of the rectangle, the color (in BGR format), and the thickness of the rectangle as parameters.

-> Finally, the modified image with rectangles around the detected faces is displayed using cv2.imshow() function.

-> The loop continues until the user presses the "Esc" key, as indicated by the condition if k==27.

-> Once the loop is terminated, the webcam is released using cap.release().

In summary, the provided code uses the Haar cascade classifier from ​OpenCV to detect faces in real-time video captured from the webcam. Detected faces are highlighted by drawing rectangles around them.
