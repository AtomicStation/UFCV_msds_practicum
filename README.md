# Unconventional Fitness Computer Vision - Mace Action Detection

## Description

A lot of current, popular fitness modalities deal with movements that are either up and down (squats, deadlifts) or front and back (bench press). Not a lot of exercises deal with side to side movements. The steel mace is an offset weight on a long handle, which allows for unique opportunities. Steel mace training provides enhanced grip strength, improved core strength and stabilization, increased range of motion, better shoulder health, and fun!

<img src="https://imgur.com/ZRirD4e.gif">

The offset nature of the weight means that momentum is used during the swings. The "float" means that the steel mace swing can also be used to train strength-endurance. Endurance activities like running have technologies that utilize GPS tracking and time, which results in accurate metrics for assessing training volume. For steel mace swings, time and swing repetitions are required for volume (swings per minute, swings per hour, etc). However, for long sessions, keeping track of swing repetitions becomes nearly impossible.

This project was designed with this problem in mind: using computer vision techniques to count reps for steel mace swings.

Currently, the project uses OpenCV and MediaPipe pose estimation data to train a LSTM RNN model to detect swings.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)

## Installation

Project requires Jupyter Notebook access.

This project imports the following libraries:
- cv2 (OpenCV)
- mediapipe (MediaPipe)
- tensoflow.keras (TensorFlow)
- numpy
- matplotlib
- scipi

## Usage

A video is just a series of images shown frame by frame:

<img src="https://imgur.com/a9qbzVb.png">

Combined, these frames create the illusion of motion:

<img src="https://imgur.com/ZRirD4e.gif">

OpenCV handles the videos, and MediaPipe detects and generates landmarks. These landmarks are used to train the model and detect actions.

<img src="https://imgur.com/N89Ib63.png">

This project uses the Pose library from MediaPipe, with the following landmarks:

<img src="https://imgur.com/gCGDZx0.png">

Currently, training is done by using OpenCV and MediaPipe to generate categorized actions. Each action is a series of 30 frames.

<img src="https://imgur.com/sv4dBQ7.png">

For example, the "hold" action could have frames that look like these:

<img src="https://imgur.com/vOvkI04.png">

And the "swing" action could have frames that look like these:

<img src="https://imgur.com/e7PJVDa.png">

Each action has 30 sets of 30 frames

<img src="https://imgur.com/0jOBKas.png">

Each frame is transformed into an array using MediaPipe landmarks

<img src="https://imgur.com/pyUn0io.png">

### Ideas for future implementations.

Instead of training the model with a specific video, any video can be used with a specific frame identifying the "hold" action:

<img src="https://imgur.com/tuM6Ana.png">

<img src="https://imgur.com/YqSWBfY.png">

## Credits

This project uses Nicholas Renotte's excellent video tutorials as a starting point.

[AI Pose Estimation with Python and MediaPipe | Plus AI Gym Tracker Project](https://youtu.be/06TE_U21FK4?si=fEvcyFsy5oCH_1Bi)

[Sign Language Detection using ACTION RECOGNITION with Python | LSTM Deep Learning Model](https://youtu.be/doDUihpj6ro?si=OIXOzqfqkaC-Qj7d)

## License

GNU General Public License v3.0
