---
title: "Automated Drug Dispenser for Government Hospitals"
excerpt: "An OTP-based medicine vending machine with a companion app for doctors, built to shorten dispensing queues at government hospitals. *ESP32, Flutter, IoT*"
collection: portfolio
order: 4
---

Medicine queues at Indian government hospitals are long, largely because dispensing is done by hand. This project automates that step.

* Built a Flutter app that lets doctors issue prescriptions digitally. Each prescription maps to a one-time code (OTP) given to the patient.
* Built a custom vending machine using an ESP32 and 360° servo motors. Each OTP is linked to the batch of medicines in the prescription, and the medicines are dispensed once the code is verified.
