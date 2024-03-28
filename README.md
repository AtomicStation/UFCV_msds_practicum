# Unconventional Fitness Computer Vision - Mace Action Detection

## Description

A lot of current, popular fitness modalities deal with movements that are either up and down (squats, deadlifts) or front and back (bench press). Not a lot of exercises deal with side to side movements. The steel mace is an offset weight on a long handle, which allows for unique opportunities. Steel mace training provides enhanced grip strength, improved core strength and stabilization, increased range of motion, better shoulder health, and fun!

The offset nature of the weight means that momentum is used during the swings. The "float" means that the steel mace swing can also be used to train strength-endurance. Endurance activities like running have technologies that utilize GPS tracking and time, which results in accurate metrics for assessing training volume. For steel mace swings, time and swing repetitions are required for volume (swings per minute, swings per hour, etc). However, for long sessions, keeping track of swing repetitions becomes nearly impossible.

This project was designed with this problem in mind: using computer vision techniques to count reps for steel mace swings.

Currently, the project uses OpenCV and MediaPipe pose estimation data to train a LSTM RNN model to detect swings.

## Table of Contents (Optional)

If your README is long, add a table of contents to make it easy for users to find what they need.

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)

## Installation

Project requires Jupyter Notebook access.

This project imports the following libraries:
cv2 (OpenCV)
mediapipe (MediaPipe)
tensoflow.keras (TensorFlow)
numpy
matplotlib
scipi

## Usage

Provide instructions and examples for use. Include screenshots as needed.

<img src="https://imgur.com/a9qbzVb.png">
<img src="https://imgur.com/N89Ib63.png">
<img src="https://imgur.com/gCGDZx0.png">
<img src="https://imgur.com/qMsLSDZ.png">
<img src="https://imgur.com/0jOBKas.png">
<img src="https://imgur.com/pyUn0io.png">

Ideas for future implementations.
<img src="https://imgur.com/tuM6Ana.png">
<img src="https://imgur.com/YqSWBfY.png">

## Credits

This project uses Nicholas Renotte's excellent video tutorials as a starting point.

[AI Pose Estimation with Python and MediaPipe | Plus AI Gym Tracker Project](https://youtu.be/06TE_U21FK4?si=fEvcyFsy5oCH_1Bi)

[Sign Language Detection using ACTION RECOGNITION with Python | LSTM Deep Learning Model](https://youtu.be/doDUihpj6ro?si=OIXOzqfqkaC-Qj7d)

## License

GNU General Public License v3.0
