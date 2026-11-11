---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* **B.Tech in Electronics and Telecommunication Engineering**, with Honours in Artificial Intelligence and Machine Learning, 2022–2026
  * Dwarkadas J. Sanghvi College of Engineering, Mumbai
  * CGPA: 9.16 / 10
  * Relevant coursework: Computer Architecture, Digital System Design, VLSI, Signals and Systems, Image Processing, Mobile Communication Systems, Computer Networks, Data Structures and Algorithms

Research Experience
======
* **Research Associate**, Indian Institute of Technology Bhubaneswar, Aug 2026 – present
  * Advisor: Prof. Debapratim Ghosh
  * Time-domain signal processing for antenna measurements

* **Project Assistant**, Digital Audio Processing Lab, IIT Bombay, Jan 2026 – Apr 2026
  * Advisor: Prof. Preeti Rao
  * Evaluated Apollo (ICASSP 2025) and HiFi-GAN+ (NeurIPS 2020) for bandwidth restoration of old Bollywood songs whose high-frequency content was truncated above 9 kHz. Assessed the results with mel-spectrograms, listening tests, SNR, SIR and ViSQOL, and found limited perceptual improvement along with high-frequency artifacts.
  * Reconstructed Apollo's undocumented evaluation pipeline, including codec simulation, time alignment and normalization. Resolved GPU inference issues in HiFi-GAN+ and automated batch evaluation across environments. Investigated discrepancies with Apollo's reported metrics, noting differences in evaluation dataset coverage.

* **Research Intern**, National Technical Research Organisation (NTRO), Bangalore, Jun 2025 – Aug 2025
  * Implemented atmospheric correction algorithms on Indian hyperspectral images, which improved NDVI results. Merged SWIR and VNIR images and built visualizations of them using Python and Napari.
  * Detected ships in Indian satellite images using ArcGIS Pro. Also worked on change detection of Indian borders, by extracting and comparing temporal images.

{% comment %} Publications hidden for now (paper rejected, Nov 2026). Remove the comment tags to restore.
Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
{% endcomment %}

Honors and Awards
======
* **Winner, MATLAB AI Challenge 2025**: 1st place globally, awarded $1,000 by MathWorks
* **Winner, Smart India Hackathon 2024**: awarded ₹1,00,000 by the Ministry of Education, Government of India

Projects
======
* [Top Quark Jet Tagging with Deep CNNs]({{ base_path }}/projects/top-quark-tagging/)
* [Hyperspectral Image Analysis Platform]({{ base_path }}/projects/hyperspectral-analysis/)
* [Autonomous Object Detection and Acquisition System]({{ base_path }}/projects/object-acquisition-robot/)
* [Automated Drug Dispenser for Government Hospitals]({{ base_path }}/projects/drug-dispenser/)

Technical Skills
======
* **Languages:** C++, C, Python, MATLAB, Verilog, Java, Assembly, Dart
* **ML frameworks:** PyTorch, Keras, MATLAB Deep Network Designer
* **Hardware and tools:** Vivado, Vitis HLS, hls4ml, Altium Designer, Linux, Git, Flutter

Leadership
======
* **Electronics Member**, DJS Arya (CanSat Competition team), Apr 2024 – Apr 2025
  * Designed the schematic and PCB for the GPS, I/O and power subsystems in Altium Designer.
  * Estimated subsystem power budgets and planned component placement for a compact design.
  * Field-tested wireless communication with XBee modules.
