# LRD-RB: Rotated Bounding-Box Dataset for Lunar Rockfall Detection

This repository provides the LRD-RB dataset and accompanying resources for the paper:

> **“LRD-RB: The First Large-Scale Dataset With Rotated Bounding Boxes for Automated Lunar Rockfall Detection”**  
> D. Miao, J. Yan, Z. Tu, J.-P. Barriot, IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing (JSTARS), 2025. :contentReference[oaicite:0]{index=0}

LRD-RB is, to the best of our knowledge, the first large-scale lunar rockfall dataset annotated with rotated bounding boxes (RBBs), designed to support research on automated rockfall detection and rotated small-object detection in remote sensing. :contentReference[oaicite:1]{index=1}

---

## 1. Dataset Overview

LRD-RB is built from high-resolution Narrow Angle Camera (NAC) images acquired by NASA’s Lunar Reconnaissance Orbiter (LRO). :contentReference[oaicite:2]{index=2}

Key characteristics:

- **Source sensor:** LRO NAC, near-nadir observations.
- **Spatial resolution:** Mostly around **0.5 m/pixel**, with the majority of images between **0.4 m/pixel and 1.75 m/pixel**. :contentReference[oaicite:3]{index=3}  
- **Image patches:** **11,697** cropped patches derived from **500** NAC images, suitable for deep-learning-based object detection. :contentReference[oaicite:4]{index=4}  
- **Annotations:** **58,298** lunar rockfall instances with **rotated bounding boxes (RBBs)**. :contentReference[oaicite:5]{index=5}  
- **Typical rockfall size:** Estimated diameters mainly between **2–15 m**, with most samples in the **4–7 m** range. :contentReference[oaicite:6]{index=6}  
- **Illumination & geography:** Wide variety of solar incidence/phase angles and geographic locations, including high-latitude and equatorial regions, to improve robustness under diverse illumination and terrain conditions. :contentReference[oaicite:7]{index=7}  

The dataset is split into **train / val / test** with a ratio of **8 : 1 : 1**. :contentReference[oaicite:8]{index=8}  

---

## 2. Download

The dataset is distributed as a compressed archive:

- **File name:** `LRDRB.zip`
- **Size:** (depends on your packaged file)
- **Hosting:** Baidu Netdisk

**Baidu Netdisk link (Mainland China friendly):**

- Link: `https://pan.baidu.com/s/14v0ourLgPEB-pxrow1s2QA`  
- Extraction code: `d7uv`

After downloading:

```bash
unzip LRDRB.zip
