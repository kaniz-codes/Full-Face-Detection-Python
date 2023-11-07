# Full-Face-Detection-Python
### This code captures video from the default camera, detects faces in the video frames, and prints the facial landmarks of the first detected face. Let me break down the code for you:

#### 1️⃣ Importing Libraries and Modules:
![codeimage-snippet_7](https://github.com/kaniz-codes/Full-Face-Detection-Python/assets/138873297/ee0eb3b8-1678-44c8-947e-ff741539799c)

- This code uses the OpenCV library (cv2) along with a custom module called FaceMeshDetector to perform face detection and facial landmark detection in real-time video from the default camera (usually the built-in webcam).
- cv2 is OpenCV, a library for computer vision tasks.
- "FaceMeshDetector" is a custom module for detecting facial landmarks using the Face Mesh model from OpenCV.

 #### 2️⃣ Opening the Video Capture Device:
![codeimage-snippet_7 (1)](https://github.com/kaniz-codes/Full-Face-Detection-Python/assets/138873297/4331b861-5035-4267-a428-09abf1faf85e)

- cv2.VideoCapture(0) initializes a video capture object (cap) that can access the default camera.
- These settings determine the resolution of the video that will be captured.
- In this case, the width is set to 1280 pixels, and the height is set to 720 pixels.

 #### 3️⃣ Initializing the Face Mesh Detector:
 ![codeimage-snippet_7 (2)](https://github.com/kaniz-codes/Full-Face-Detection-Python/assets/138873297/38757898-2004-4910-9b28-e1e33ef93c3b)

- An instance of the FaceMeshDetector class is created. The maxFaces parameter is set to 1, which means it will detect landmarks for only one face in the frame.

 #### 4️⃣ Capturing and Processing Video:
 ![codeimage-snippet_7 (3)](https://github.com/kaniz-codes/Full-Face-Detection-Python/assets/138873297/9798f8b7-08f8-4e25-8f30-92358527e6bf)

- cap.read() reads a frame from the video capture device (cap). The frame is stored in the img variable, and success is a boolean indicating whether the frame was successfully read.
- detector.findFaceMesh(img) processes the frame using the Face Mesh model to detect facial landmarks. The detected faces and their landmarks are returned as faces.
- cv2.imshow("Imgage", img) displays the captured frame in a window with the title "Imgage."
- cv2.waitKey(1) waits for a key press for 1 millisecond to allow the window to refresh and display the next frame.

  In summary, this code captures video from the default camera, sets the frame resolution, uses the FaceMeshDetector to detect facial landmarks, and prints the landmarks for the detected face(s) in real-time. It's a basic example of how to perform facial landmark detection using OpenCV and a custom module.

 #### 🐍 Final Code:
![codeimage-snippet_7 (4)](https://github.com/kaniz-codes/Full-Face-Detection-Python/assets/138873297/69748cab-a635-4025-86dd-95076b5cd659)


