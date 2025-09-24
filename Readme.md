<!-- Optional banner -->
<p align="center">
  <img src="./assets/hero_banner.png" alt="NewWeaponDataset" width="85%">
</p>

<h1 align="center">🔫🗡️ NewWeaponDataset</h1>
<p align="center">
  <em>Public, small-object-focused dataset for multi-class weapon detection (knife, pistol, long_gun) and hard negatives (no_weapon), curated from diverse day/night CCTV & handheld scenes with occlusions and clutter.</em>
</p>

<p align="center">
  <a href="<INSERT_ROBOFLOW_UNIVERSE_LINK>">
    <img src="https://img.shields.io/badge/Open%20in%20Roboflow-000?logo=roboflow&logoColor=white&style=for-the-badge" alt="Open in Roboflow">
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Format-YOLOv5%2Fv8-1f77b4?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-6c757d?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Hosted-Roboflow%20Universe-20c997?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Public-Yes-2ca02c?style=for-the-badge" />
</p>

---

## ⚡ At a Glance

<table>
  <tr>
    <td><b>🖼️ Images</b></td>
    <td><b>59,305</b></td>
  </tr>
  <tr>
    <td><b>🔢 Instances</b></td>
    <td><b>76,705</b> (0 empty labels)</td>
  </tr>
  <tr>
    <td><b>🏷️ Classes</b></td>
    <td><code>knife</code>, <code>long_gun</code>, <code>no_weapon</code>, <code>pistol</code></td>
  </tr>
  <tr>
    <td><b>🧰 Format</b></td>
    <td>YOLO: <code>class x_center y_center width height</code> (normalized)</td>
  </tr>
  <tr>
    <td><b>📜 License</b></td>
    <td>MIT</td>
  </tr>
  <tr>
    <td><b>☁️ Hosting</b></td>
    <td><a href="<INSERT_ROBOFLOW_UNIVERSE_LINK>">Roboflow Universe (Public)</a></td>
  </tr>
</table>

---

## 🧪 Split Mix

<p>
  <img src="https://img.shields.io/badge/Train-82.76%25-228be6?style=flat-square" />
  <img src="https://img.shields.io/badge/Valid-12.73%25-845ef7?style=flat-square" />
  <img src="https://img.shields.io/badge/Test-4.51%25-15aabf?style=flat-square" />
</p>

<pre>
Train  [███████████████████████████████████████░░] 82.76% (49,079)
Valid  [██████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░] 12.73% (7,552)
Test   [███░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░]  4.51% (2,674)
</pre>

---

## 🎯 Class Mix (All Splits)

<p>
  <img src="https://img.shields.io/badge/knife-13,010_(16.96%25)-e74c3c?style=for-the-badge" />
  <img src="https://img.shields.io/badge/long_gun-22,964_(29.94%25)-8e44ad?style=for-the-badge" />
  <img src="https://img.shields.io/badge/no_weapon-12,141_(15.83%25)-95a5a6?style=for-the-badge" />
  <img src="https://img.shields.io/badge/pistol-28,590_(37.27%25)-f1c40f?style=for-the-badge" />
</p>

> Class distribution chart: `./assets/class_distribution.png`  
> (Copy from `/home/constantin/Doctorat/YoloLib/Utils/Scripts/merged_dataset/class_distribution.png` into `./assets/`.)

---

## 🗂️ Structure & Labels

- **Annotation format:** `class_id x_center y_center width height` (all normalized to `[0,1]`)
- **Index map:**
