# Math Gesture AI

## Overview

**Math Gesture AI** is an AI-powered application that recognizes hand gestures and interprets them into mathematical operations. The project leverages TensorFlow and OpenCV to detect hand gestures in real-time and translates them into actions such as addition, subtraction, multiplication, and division.

## Features

- **Real-time Hand Gesture Recognition**: Uses TensorFlow models to identify and classify hand gestures.
- **AI-Powered Problem Solving**: Integrates Google Generative AI (Gemini Model) to solve mathematical problems based on recognized gestures.
- **User-Friendly Interface**: An intuitive interface for interacting with the AI system.
- **Cross-Platform Compatibility**: Works on multiple platforms including Windows, macOS, and Linux.

### Prerequisites

- Python 3.8+
- TensorFlow 2.x
- OpenCV 4.x
- Streamlit 1.x
- Google Generative AI API Key

## Gesture Guide
- Draw Gesture: Show the "Index Finger" (fingers = [0, 1, 0, 0, 0]) to draw.
- Erase Gesture: Show the "Thumb" (fingers = [1, 0, 0, 0, 0]) to erase the canvas.
- Solve Gesture: Show the "Four Fingers Up" (fingers = [1, 1, 1, 1, 0]) to send the drawing to the AI for problem-solving.

The system will display the recognized operation on the screen and provide an AI-generated answer to the problem.
## Project Structure
main.py: The entry point for running the application.
models/: Contains pre-trained models used for gesture recognition.
utils/: Utility scripts for processing images and managing the dataset.
README.md: Project documentation.
requirements.txt: List of dependencies required to run the project.
