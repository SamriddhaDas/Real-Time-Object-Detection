Real-Time Object Detection Web App
This project is a simple, self-contained web application that performs real-time object detection using your computer's webcam. It leverages the power of TensorFlow.js and a pre-trained COCO-SSD model to identify and label common objects in a live video stream, directly in your web browser.

Features
Real-Time Detection: Identifies objects in a live webcam feed.

Bounding Boxes: Draws boxes around detected objects.

Class Labels: Displays the name of the detected object (e.g., "person", "laptop", "cell phone").

Confidence Scores: Shows the model's confidence level for each detection as a percentage.

Object Counting: Provides a live count of the total number of objects detected in the frame.

Responsive Design: The interface adapts to different screen sizes.

Zero Installation: Runs entirely in the browser with no need for backend servers or complex setup.

How It Works
The application is built using a single index.html file and relies on the following core technologies:

HTML: Provides the basic structure of the web page.

Tailwind CSS: Used for modern and responsive styling.

TensorFlow.js: A powerful open-source library for machine learning in JavaScript. It allows us to run the object detection model directly in the browser.

COCO-SSD Model: A pre-trained object detection model that can recognize 90 common object classes. The model is loaded directly from TensorFlow's model repository.

The application's logic follows these steps:

Loads the pre-trained COCO-SSD model.

Requests access to the user's webcam.

Once access is granted, it displays the video feed.

In a continuous loop, it captures frames from the video, passes them to the model for prediction, and draws the results (bounding boxes and labels) onto a canvas element overlaid on top of the video.

Requirements
A modern web browser (e.g., Google Chrome, Mozilla Firefox, Microsoft Edge).

A webcam connected to your computer.

Usage
Save the code from the index.html file provided in the project.

Open the index.html file directly in your web browser.

When prompted, grant the browser permission to access your webcam.

The application will load the model (you'll see a loading indicator).

Point your webcam at different objects to see the real-time detection in action!

Credits
This project was made possible by the following open-source libraries:

TensorFlow.js

COCO-SSD Model for TensorFlow.js

Tailwind CSS
