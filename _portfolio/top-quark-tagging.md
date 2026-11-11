---
title: "Top Quark Jet Tagging with Deep CNNs"
excerpt: "**Winner, MATLAB AI Challenge 2025 (1st place globally).** A ResNeXt + squeeze-and-excitation CNN that separates top-quark jets from QCD background. *MATLAB Deep Network Designer, FPGA/HLS*"
collection: portfolio
order: 1
---

Built for the MATLAB AI Challenge 2025, where it placed first worldwide.{% comment %} Hidden: paper rejected (Nov 2026). The work was later extended into a [manuscript now under review at *Neural Networks*](/publication/2026-09-20-modified-resnext).{% endcomment %}

* Built a CNN classifier in MATLAB Deep Network Designer to identify top-quark jets from QCD background, using jet energy and momentum values from CERN's open dataset on Zenodo.
* Designed a new architecture that combines ResNeXt blocks with squeeze-and-excitation (SE) channel attention in the intermediate stages, followed by late fusion of global features to pick out the most relevant statistics.
* Shaped the architecture around the spatial and channel structure of the jet data, with FPGA deployment in mind.
* Reached **90.87% accuracy**, **ROC AUC of 0.968** and **PR AUC of 0.971**.
