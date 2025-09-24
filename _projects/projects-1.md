---
title: "Neural Compression for 3D Volumes"
excerpt: "Compact, learned compression for large CT/MRI and scientific datasets. TINC-Plus uses a tree-structured neural model with adaptive detail and lightweight calibration to preserve quality while dramatically reducing storage, with simple one-file exports"
collection: portfolio
---

# Overview
**TINC-Plus** is a system for shrinking very large 3D images and volumes (e.g., CT/MRI scans, scientific datasets, giant TIFF stacks) into **tiny, portable files**—while keeping what matters visible and measurable.

# Description
Instead of storing every single value, TINC-Plus learns a **compact recipe** for the data. When you need it back, it **redraws** the volume from that recipe, preserving structure and detail that humans and downstream tools care about.

# Model Architecture
- **Octree partitioning:** The volume is recursively split into 3D blocks (an octree). Coarse nodes cover large regions; deeper leaves focus on fine detail.
- **Tree-structured MLPs:** Each node owns a tiny MLP that maps coordinates in its region to predicted values. Parent outputs provide a coarse basis; children refine it, adding detail progressively down the tree.
- **Hierarchical decoding:** During decompression, we traverse the tree to generate predictions, then assemble leaf outputs back into the full volume.
- **Adaptive parameter allocation:** Model capacity is distributed across nodes based on data variability or residual error, giving complex regions more parameters and simple regions fewer.
- **Lightweight calibration:** After reconstruction, small affine corrections (global or per-leaf) nudge predictions closer to the original, improving fidelity with minimal storage cost.

# Key Features
- **Adaptive Detail:** Complex areas get more modeling effort; simple areas use less.  
- **Calibration:** Global and per-region corrections polish the reconstruction quality.  
- **Lean Storage:** Space-efficient formats (like 8-bit or half-precision) and an option to save the whole model as **one compact archive**.  
- **Transparent Metrics:** Progress, quality, and timing are logged for easy comparison.

# Benefits
- **Smaller Files:** Dramatically reduced storage and faster sharing.  
- **High Fidelity:** Preserves structures and textures important for analysis.  
- **Practical Runtime:** Runs on common GPUs.

# Screeenshots


**Tree-Structured MLPs in TINC:**
<br/>
<img src='https://YasinDanesh.github.io/images/TINCP_Struct.png' alt='TINCPlus Structure' style="margin-bottom:15px; width: 100%">

**TINC-Plus PSNR/SSIM comparing to other mothods:**
<br/>
<img src='https://YasinDanesh.github.io/images/TINCP_Table.png' alt='PSNR/SSIM table' style="margin-bottom:15px; width: 100%">
<br/>
<br/>

For full code and further details, visit [TINC-Plus project](https://github.com/YasinDanesh/TINC)