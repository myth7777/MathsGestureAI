MathsGestureAI
MathsGestureAI is a cutting-edge application designed to interpret hand gestures and solve mathematical problems in real-time. This project combines computer vision, AI, and interactive UI elements to create an intuitive experience where users can draw mathematical expressions in the air and instantly receive solutions.

Project Overview
MathsGestureAI aims to make math problem-solving more interactive and accessible by using hand gestures as input. The application captures hand movements through a webcam, processes the gestures to recognize mathematical symbols, and then uses AI to solve the problem. The result is displayed in a user-friendly interface.

Features
1. Real-Time Hand Gesture Detection
Tool: OpenCV, cvzone
Functionality: The application captures real-time video feed from a webcam and uses the HandDetector class from cvzone to detect hand landmarks. It can track up to one hand at a time with high accuracy, ensuring smooth interaction.
2. Gesture-Based Drawing
Tool: OpenCV, NumPy
Functionality: Users can draw mathematical symbols and expressions in the air using their index finger. The application interprets these gestures and renders them onto a virtual canvas.
3. AI-Powered Problem Solving
Tool: Google Generative AI
Functionality: Once a mathematical expression is drawn, it can be sent to the AI model, which interprets the drawing and provides the solution. The integration with Google Generative AI ensures accurate and reliable problem-solving capabilities.
4. Interactive User Interface
Tool: Streamlit
Functionality: The application features an interactive and responsive UI, where users can start or stop the hand gesture detection, view the live feed, and see the AI-generated solutions. Streamlit makes the interface intuitive and easy to use.
Tools and Libraries
OpenCV: For capturing video feed and processing images.
cvzone: Simplifies the implementation of hand tracking and gesture recognition.
Google Generative AI: Provides AI-based interpretation and solution generation for mathematical problems.
Streamlit: Used for creating an interactive web-based interface.
PIL (Pillow): For handling image conversions when interacting with the AI model.
NumPy: Used for efficient image and data processing.
How It Works
Webcam Initialization:

The application initializes the webcam to capture real-time video feed.
The frame is processed to detect hand gestures.
Hand Detection and Tracking:

The HandDetector class from cvzone is used to detect the position and movement of the hand.
Specific gestures, such as holding up a finger or swiping, are recognized and used for different functionalities like drawing or erasing.
Drawing on Canvas:

The application allows users to draw on a virtual canvas by moving their fingers in the air.
The drawn expression is dynamically updated and displayed on the interface.
AI Interpretation and Solution:

Once the expression is complete, it can be sent to the Google Generative AI model.
The AI interprets the drawing, solves the problem, and returns the result, which is then displayed on the interface.
User Interaction:

Streamlit provides an easy-to-use interface where users can control the application, view the live feed, and read the AI-generated solution.
