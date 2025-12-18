# LRD-RB: Rotated Bounding-Box Dataset for Lunar Rockfall Detection

This repository provides the LRD-RB dataset and accompanying resources for the paper:

> **“LRD-RB: The First Large-Scale Dataset With Rotated Bounding Boxes for Automated Lunar Rockfall Detection”**  
> Dingruibo Miao, Jianguo Yan, Zhigang Tu, and Jean-Pierre Barriot  
> IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing (JSTARS), Vol. 18, 2025.  
> DOI: 10.1109/JSTARS.2025.3582117

LRD-RB is, to the best of our knowledge, the first large-scale lunar rockfall dataset annotated with rotated bounding boxes (RBBs), designed to support research on automated rockfall detection and rotated small-object detection in remote sensing.

---

## 1. Dataset Overview

LRD-RB is built from high-resolution Narrow Angle Camera (NAC) images acquired by NASA’s Lunar Reconnaissance Orbiter (LRO).

Key characteristics:

- **Source sensor:** LRO NAC, near-nadir observations.
- **Number of source images:** 500 NAC images carefully selected by planetary science experts.
- **Image patches:** 11,697 cropped patches (1024 × 1024 pixels) suitable for deep learning–based object detection.
- **Annotations:** 58,298 lunar rockfall instances with **rotated bounding boxes (RBBs)**.
- **Diversity:** 
  - Wide range of solar incidence and phase angles.
  - Broad geographic coverage, including high-latitude and equatorial regions.
  - Various terrain types (mare, highlands, crater rims), providing rich variability for model training.
- **Data Format:**
  - Each image patch has a corresponding text annotation file. Each line in an annotation file contains: (x1 y1 x2 y2 x3 y3 x4 y4 category). (x1, y1), ..., (x4, y4) are the four vertices of the rotated bounding box (pixel coordinates). category is the class label (e.g., rockfall).
The dataset is split into **train / val / test** with a ratio of **8 : 1 : 1**.

---

## 2. Download

The dataset is distributed as a compressed archive:

- **File name:** `LRDRB.zip`
- **Hosting (Mainland China friendly):** Baidu Netdisk

**Baidu Netdisk link**

- Link: `https://pan.baidu.com/s/14v0ourLgPEB-pxrow1s2QA`  
- Extraction code: `d7uv`


## 3. Citation
```bash
@article{miao2025lrd,
  title   = {LRD-RB: The First Large-Scale Dataset With Rotated Bounding Boxes for Automated Lunar Rockfall Detection},
  author  = {Miao, Dingruibo and Yan, Jianguo and Tu, Zhigang and Barriot, Jean-Pierre},
  journal = {IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing},
  volume  = {18},
  year    = {2025},
  doi     = {10.1109/JSTARS.2025.3582117}
}

