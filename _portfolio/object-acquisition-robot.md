---
title: "Autonomous Object Detection and Acquisition System"
excerpt: "A Raspberry Pi 5 robot that uses an upward-facing fisheye camera to track a thrown ball and drive toward it. *Python, OpenCV, Raspberry Pi*"
collection: portfolio
order: 3
---

A Mecanum-wheel robot that watches the space above it with an upward-facing 170° fisheye camera and moves toward a thrown ball. All processing runs on a Raspberry Pi 5, at about 60 FPS on 192×192 frames, with no hardware acceleration.

* Detected the ball with HSV color masking and two sets of contour thresholds, one for a nearby ball and one for a small, distant one in the air. A multi-frame confirmation step rejects false positives.
* Implemented two control modes. Continuous tracking uses a Kalman filter and a PD controller with a correction for fisheye distortion. Direction prediction fits a line to recent ball positions and commits to a one-second drive in that direction.
