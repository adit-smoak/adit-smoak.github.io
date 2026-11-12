---
title: "Top Quark Jet Tagging with Deep CNNs"
excerpt: "**Winner, MATLAB AI Challenge 2025 (1st place globally).** A ResNeXt + squeeze-and-excitation CNN that separates top-quark jets from QCD background. *MATLAB Deep Network Designer, FPGA/HLS*"
collection: portfolio
order: 1
---

Built for the MATLAB AI Challenge 2025, where it placed first worldwide.{% comment %} Hidden: paper rejected (Nov 2026). The work was later extended into a [manuscript now under review at *Neural Networks*](/publication/2026-09-20-modified-resnext).{% endcomment %}

A top quark decays almost as soon as it is produced, leaving a narrow spray of particles (a jet) in the detector. The goal was to separate these jets from the much more common jets produced by ordinary QCD processes, using CERN's open dataset on Zenodo.

I turned each jet into an image. The 35 most energetic particles are placed on a 37×37 grid of pseudorapidity and azimuthal angle, and every pixel stores 12 statistics about the particles that land in it, such as their count, total energy and transverse momentum, and higher moments like variance and skewness. Each image is rotated and flipped to a common orientation, so the network does not learn the jet's arbitrary direction, and then normalized pixel by pixel.

The classifier is a custom CNN built in MATLAB Deep Network Designer. It combines ResNeXt-style grouped convolutions with squeeze-and-excitation blocks, which learn how much weight to give each channel. A few whole-jet statistics are added just before the fully connected layers. Grouped convolutions also keep the computation small and easy to parallelize, which was chosen with FPGA deployment in mind. The final model reached **90.87% accuracy**, a **ROC AUC of 0.968** and a **PR AUC of 0.971**.
