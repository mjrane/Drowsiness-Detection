# Drowsiness-Detection using Haar- Cascade method
A Haar Cascade is based on “Haar Wavelets” which Wikipedia defines as: A sequence of rescaled “square-shaped” functions which together form a wavelet family or basis.
It is based on the Haar Wavelet technique to analyze pixels in the image into squares by function. This uses machine learning techniques to get a high degree of accuracy from what is called “training data”. This uses “integral image” concepts to compute the “features” detected. Haar Cascades use the Adaboost learning algorithm which selects a small number of important features from a large set to give an efficient result of classifiers.

## Steps to work:
### Step 1: Gathering libraries(Python: import cv2, potentially others)
•	import cv2: Imports the OpenCV library, essential for image processing tasks like face detection.
### Step 2: Loading/Reading files (Python: cv2.imread(), cv2.imshow())
•	cv2.imread(): Loads an image containing faces (typically a file path or a pre-captured image).
•	cv2.imshow(): Displays the loaded image on your screen, allowing you to visualize it.
### Step 3: Run the classifier (Python: cv2.CascadeClassifier(), detectMultiScale())
•	cv2.CascadeClassifier(): Creates a pre-trained facial feature detector using OpenCV's built-in cascade classifier.
•	detectMultiScale(): Applies the detector to the image, searching for features that suggest the presence of faces. If faces are found, it returns the coordinates (x, y, width, height) for each detected face.
### Step 4: Zooming In (Optional) (Python: ROI creation, eye detection)
•	ROI creation (optional): If you want to focus on specific aspects of detected faces, you can create a Region of Interest (ROI) using the face coordinates. This allows you to perform additional processing, such as eye detection, within that specific area.
•	Eye detection (optional): You could potentially apply another detection process, like eye detection, within the created ROI.
### Step 5: From Images to Videos  (Real-time video using cv2.VideoCapture()
•	cv2.VideoCapture() : To extend from static images to real-time video, you can use this function to access a video stream (e.g., from your webcam). Then, you'd iterate through video frames, applying the face detection process to each frame.


