---
title: "Modified Aggregated Residual Network with Squeeze and Excite Block for Top Quark Tagging"
collection: publications
published: false   # hidden for now (paper rejected, Nov 2026); delete this line to restore the page
category: manuscripts
permalink: /publication/2026-09-20-modified-resnext
excerpt: 'A ResNeXt-based CNN with squeeze-and-excitation channel attention for distinguishing top-quark jets from QCD background, designed with FPGA deployment in mind.'
date: 2026-09-20
venue: 'Neural Networks'
status: 'Under review'   # remove this line once the paper is accepted; the site will then say "Published in"
citation: 'Adit Shah and Satishkumar Chavan. (2026). &quot;Modified Aggregated Residual Network with Squeeze and Excite Block for Top Quark Tagging.&quot; <i>Neural Networks</i>. Under review.'
---

Identifying jets that originate from top quarks, against a much larger background of QCD jets, is a core classification task in collider physics. This work proposes a modified aggregated residual network (ResNeXt) for the task. Squeeze-and-excitation (SE) channel attention is placed in the intermediate stages, and global features are fused late in the network. The architectural changes take the spatial and channel structure of jet data into account, and aim to maximize parallelism for deployment on FPGAs.

The work began as my winning entry to the [MATLAB AI Challenge 2025](/projects/top-quark-tagging/), and was extended with FPGA synthesis experiments across several high-level synthesis toolchains.
