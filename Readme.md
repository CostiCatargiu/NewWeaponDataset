<!-- Optional banner -->
<p align="center">
  <img src="./assets/hero_banner.png" alt="NewWeaponDataset" width="85%">
</p>

<h1 align="center">🔫🗡️ NewWeaponDataset</h1>
<p align="center">
  <em>Public, small-object-focused dataset for multi-class weapon detection (knife, pistol, long_gun) and hard negatives (no_weapon). Curated from diverse CCTV/handheld sources across day/night, occlusions, motion blur, and clutter—built to stress-test real surveillance models.</em>
</p>

<p align="center">
  <a href="https://universe.roboflow.com/gundetectiondataset/nogun/dataset/2">
    <img src="https://img.shields.io/badge/Open%20NoGun%20Dataset-111?logo=roboflow&logoColor=white&style=for-the-badge" alt="Open NoGun Dataset" />
  </a>
  <a href="https://app.roboflow.com/gundetectiondataset/weapondataset-oi2g3/8">
    <img src="https://img.shields.io/badge/Open%20WeaponDataset%20v8-111?logo=roboflow&logoColor=white&style=for-the-badge" alt="Open WeaponDataset v8" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Format-YOLOv5%2Fv8-1f77b4?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-6c757d?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Hosted-Roboflow%20Universe-20c997?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Public-Yes-2ca02c?style=for-the-badge" />
</p>

---

## ⚡ At a Glance (Summary)

<table>
  <tr>
    <td><b>🖼️ Images</b></td><td><b>59,305</b></td>
  </tr>
  <tr>
    <td><b>🔢 Instances</b></td><td><b>76,705</b> &nbsp;•&nbsp; <i>0 empty labels</i></td>
  </tr>
  <tr>
    <td><b>🏷️ Classes</b></td>
    <td><code>knife</code>, <code>long_gun</code>, <code>no_weapon</code>, <code>pistol</code> &nbsp; | &nbsp; Index map: <code>0: knife</code>, <code>1: long_gun</code>, <code>2: no_weapon</code>, <code>3: pistol</code></td>
  </tr>
  <tr>
    <td><b>🧰 Format</b></td>
    <td>YOLO — <code>class_id x_center y_center width height</code> (normalized to [0,1])</td>
  </tr>
  <tr>
    <td><b>🧪 Split Mix</b></td>
    <td>Train <b>82.76%</b> (49,079) • Valid <b>12.73%</b> (7,552) • Test <b>4.51%</b> (2,674)</td>
  </tr>
  <tr>
    <td><b>🎯 Class Mix</b></td>
    <td>
      <img src="https://img.shields.io/badge/knife-13,010_(16.96%25)-e74c3c?style=for-the-badge" />
      <img src="https://img.shields.io/badge/long_gun-22,964_(29.93%25)-8e44ad?style=for-the-badge" />
      <img src="https://img.shields.io/badge/no_weapon-12,141_(15.83%25)-95a5a6?style=for-the-badge" />
      <img src="https://img.shields.io/badge/pistol-28,590_(37.27%25)-f1c40f?style=for-the-badge" />
    </td>
  </tr>
  <tr>
    <td><b>☁️ Hosting</b></td>
    <td>
      <a href="https://universe.roboflow.com/gundetectiondataset/nogun/dataset/2">Roboflow Universe: NoGun</a> &nbsp;•&nbsp;
      <a href="https://app.roboflow.com/gundetectiondataset/weapondataset-oi2g3/8">Roboflow App: WeaponDataset v8</a>
    </td>
  </tr>
</table>

---

## 🧾 About the Dataset & This Work

This dataset was assembled to address the gap between **lab benchmarks** and **real security footage**. We focused on:
- **Small objects & distance**: many samples feature tiny targets, partials, and heavy occlusion.
- **Hard negatives (`no_weapon`)**: diverse non-weapon scenes (phones, umbrellas, tools, hands, reflections) to control false positives in production.
- **Varied domains**: indoor/outdoor, day/night, CCTV angles, motion blur, and clutter.

**Annotation protocol** follows YOLO normalized boxes with consistent class taxonomy (`knife`, `long_gun`, `pistol`, `no_weapon`). Splits were made to preserve distribution while avoiding leakage, and the set was de-duplicated and QA’d to remove corrupt/empty labels (now **0**).

This work underpins research into **robust real-time weapon detection**, emphasizing **tiny-object recall** without exploding false positives. We encourage comparing backbones (YOLOv8/11/12), tuning anchor-free heads, and experimenting with pre-processing (e.g., CLAHE/adaptive equalization) when appropriate for your deployment domain.

> 📊 Class distribution chart: `./assets/class_distribution.png`  
> Copy from: `/home/constantin/Doctorat/YoloLib/Utils/Scripts/merged_dataset/class_distribution.png` → `./assets/` to render here.

---

## 🚀 Quick Start (YOLOv8)

```bash
pip install ultralytics
yolo task=detect mode=train model=yolov8n.pt data=data.yaml epochs=50 imgsz=640
