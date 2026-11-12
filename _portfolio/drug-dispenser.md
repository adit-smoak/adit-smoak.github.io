---
title: "Automated Drug Dispenser for Government Hospitals"
excerpt: "An OTP-based medicine vending machine with a companion app for doctors, built to shorten dispensing queues at government hospitals. *ESP32, Flutter, IoT*"
collection: portfolio
order: 4
---

Medicine queues at Indian government hospitals are long, largely because medicines are handed out manually at a counter. This project is a small-scale prototype that automates that step.

A doctor writes the prescription in a Flutter app instead of on paper. The app links the prescription to a one-time code (OTP), which the patient takes to a dispensing machine. The machine is built around an ESP32 microcontroller. When the patient enters the code and it is verified, the machine uses 360° servo motors to drop every medicine in that prescription.
