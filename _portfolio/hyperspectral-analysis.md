---
title: "Hyperspectral Image Analysis Platform"
excerpt: "**Winner, Smart India Hackathon 2024.** End-to-end hyperspectral pipeline covering atmospheric correction, denoising and GAN-based anomaly detection. *Python, PyTorch, Py6S*"
collection: portfolio
order: 2
---

Built as a team for the Smart India Hackathon 2024. We won first place at the finals at IIT Roorkee, with an award of ₹1,00,000 from the Ministry of Education, Government of India.

A hyperspectral image records a full spectrum at every pixel instead of just red, green and blue, so materials that look the same in an ordinary photo can still be told apart. Our task was an end-to-end pipeline that finds anomalies in these images: pixels whose spectra do not match their surroundings.

Raw images need cleaning before detection is reliable. We corrected for the atmosphere with Py6S (a radiative-transfer model) and a flat-field method, which removes the effect of light being scattered and absorbed by gases on its way to the sensor. We then reduced noise by fine-tuning QRNN3D, a network designed for hyperspectral denoising, on several types of noise. For the detection step we implemented a semi-supervised GAN from a research paper whose code had not been released, so the model had to be rebuilt and trained from the paper's description alone.
