<h2 align="center">Advanced Pixel Diffusion Model with Guided Sparse Global Refinement</h2>

<p align="center">
  Weiyi You &middot;
  Jinhua Zhang &middot;
  Xingyu Zhou &middot;
  Wei Long &middot;
  Junyu Lou &middot;
  <a href="https://scholar.google.com/citations?user=-kSTt40AAAAJ">Shuhang Gu</a><sup>†</sup>
</p>

<p align="center">
  University of Electronic Science and Technology of China
</p>

<p align="center">
  <sup>†</sup> Corresponding author
</p>

<p align="center">
  <a href="https://arxiv.org/abs/2609.00798">
    <img src="https://img.shields.io/badge/arXiv-2609.00798-b31b1b.svg" alt="arXiv">
  </a>
  <a href="https://github.com/CVL-UESTC/PixSGR">
    <img src="https://img.shields.io/github/stars/CVL-UESTC/PixSGR?style=social" alt="GitHub stars">
  </a>
  <a href="https://huggingface.co/CVLUESTC/PixSGR">
    <img src="https://img.shields.io/badge/🤗%20Hugging%20Face-CVLUESTC%2FPixSGR-yellow" alt="Hugging Face">
  </a>
</p>

## Overview

PixSGR is an efficient pixel-space diffusion framework for high-fidelity image
generation. It starts from a supervised low-channel bottleneck that captures the
low-dimensional manifold of natural images, then progressively expands the
channel dimensionality and spatial resolution to recover fine-grained structures.
During spatial refinement, coarse-scale attention maps preselect globally relevant
interactions for fine-scale sparse attention, enabling non-local refinement without
the quadratic cost of dense attention.

On ImageNet, PixSGR achieves FID scores of **1.51** at **256 &times; 256** and
**1.60** at **512 &times; 512**.

## Framework

<p align="center">
  <img src="asset/framework.png" width="95%" alt="Overview of the PixSGR architecture">
</p>

<p align="center">
  <em>PixSGR couples cross-scale token scoring with guided sparse attention and convolutional upsampling.</em>
</p>


## Contact

For questions or collaborations, contact
[Weiyi You](mailto:weiyiyou.ywy@gmail.com).

If you find this work useful, please consider starring the repository.
