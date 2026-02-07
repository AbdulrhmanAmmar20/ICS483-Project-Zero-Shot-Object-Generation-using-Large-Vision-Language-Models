# ICS483-Project-Zero-Shot-Object-Generation-using-Large-Vision-Language-Models
We’re reimplementing AnyDoor, a zero-shot diffusion model that “teleports” a chosen object into a new scene at a user-specified spot. It preserves identity (logos, textures, lighting) via a Detail Extractor. We’ll test robustness on “impossible” geometry placements and improve inference for user-captured photos.

## Authors
 - Paper Authors:
   Xi Chen, Lianghua Huang, Yu Liu, Yujun Shen, Deli Zhao, and Hengshuang Zhao.

- Our Team:
  Abdulrahman Ammar, Omar Bahaeldin Abdalla, Mohammed Al Sheqaih

## Project Title
Zero-Shot Object Teleportation via High-Fidelity Image Customization

## Problem Statement / Idea
Traditional image editing and inpainting methods struggle to insert objects into new scenes without losing their visual identity, context, or texture consistency. For instance, when blending a specific handbag or toy into a different background, existing methods often fail to preserve high-frequency details (logos, reflections, materials) or adapt to scene lighting and geometry. The challenge is to perform object-level customization without fine-tuning, enabling zero-shot transfer for unseen objects and environments.

This project addresses that issue by reimplementing and extending AnyDoor (CVPR 2024), a diffusion-based framework capable of “teleporting” an arbitrary object into a new scene at a user-specified location, while maintaining its distinctive attributes.

## Brief Project Overview
This project explores zero-shot object-level image generation through the reimplementation of AnyDoor, a state-of-the-art diffusion framework for high-fidelity object teleportation. The model operates without fine-tuning and integrates a Detail Extractor module to preserve detailed object identity and lighting consistency that standard inpainting often degrades.

We will evaluate the model’s robustness on challenging (“impossible”) geometry placements—such as mounting rigid objects on soft or irregular surfaces—and enhance the inference pipeline for greater adaptability to custom, user-captured photos. Evaluation datasets include VITON-HD, DreamBench, and a small custom dataset of 30–50 personally photographed items (like backpacks, shoes, tools) to demonstrate real-world performance.

Reference Paper: AnyDoor: Zero-Shot Object-Level Image Customization (CVPR 2024)
Reference Repository: https://github.com/ali-vilab/AnyDoor
