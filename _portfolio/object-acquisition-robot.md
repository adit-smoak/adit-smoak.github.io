---
title: "Autonomous Object Detection and Acquisition System"
excerpt: "A Raspberry Pi 5 robot that uses an upward-facing fisheye camera to track a thrown ball and drive toward it. *Python, OpenCV, Raspberry Pi*"
collection: portfolio
order: 3
---

A small robot with a camera pointing straight up. When someone throws a ball over it, the robot works out where the ball is heading and drives there. It uses Mecanum wheels, which let it move in any direction without turning first.

Everything runs on a Raspberry Pi 5 with no hardware accelerator. A 170° fisheye camera captures 192×192 frames, which OpenCV processes at about 60 FPS. The ball is found by its colour (HSV masking) and the shape of its outline. There are separate thresholds for a large ball close to the camera and a small one far up in the air, and a detection only counts once it appears in several frames in a row.

The robot has two control modes. The first tracks the ball continuously: a Kalman filter smooths its position and a PD controller steers, with a correction for the fisheye lens distortion. The second fits a line to the ball's last few positions, predicts its direction, and commits to a one-second drive that way.
