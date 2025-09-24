<!-- Optional banner -->
<p align="center">
  <img src="./assets/hero_banner.png" alt="NewWeaponDataset" width="85%">
</p>

<h1 align="center">🔫🗡️ NewWeaponDataset</h1>
<p align="center">
  <em>Public, small-object-focused dataset for multi-class weapon detection (knife, pistol, long_gun) and hard negatives (no_weapon), curated from diverse day/night CCTV & handheld scenes with occlusions and clutter.</em>
</p>

<p align="center">
  <a href="https://universe.roboflow.com/gundetectiondataset/nogun/dataset/2">
    <img src="https://img.shields.io/badge/Open%20NoGun%20Dataset-0d1117?logo=roboflow&logoColor=white&style=for-the-badge&color=A5D6A7" alt="Open NoGun Dataset on Roboflow">
  </a>
  <a href="https://app.roboflow.com/gundetectiondataset/weapondataset-oi2g3/8">
    <img src="https://img.shields.io/badge/Open%20WeaponDataset%20v8-0d1117?logo=roboflow&logoColor=white&style=for-the-badge&color=90CAF9" alt="Open WeaponDataset v8 on Roboflow">
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Format-YOLOv5%2Fv8-0d1117?style=for-the-badge&color=89C2FF" />
  <img src="https://img.shields.io/badge/License-MIT-0d1117?style=for-the-badge&color=CFCFCF" />
  <img src="https://img.shields.io/badge/Hosted-Roboflow%20Universe-0d1117?style=for-the-badge&color=7EE0C3" />
  <img src="https://img.shields.io/badge/Public-Yes-0d1117?style=for-the-badge&color=F9D36F" />
</p>

---

## ⚡ At a Glance

<table>
  <tr>
    <td><b>🖼️ Images</b></td>
    <td>
      <img src="https://img.shields.io/badge/59,305-0d1117?style=flat-square&color=00C2A8&labelColor=0d1117" />
    </td>
  </tr>
  <tr>
    <td><b>🔢 Instances</b></td>
    <td>
      <img src="https://img.shields.io/badge/76,705-0d1117?style=flat-square&color=FF9F43&labelColor=0d1117" />
      <img src="https://img.shields.io/badge/empty_labels-0-0d1117?style=flat-square&color=6CFF8D&labelColor=0d1117" />
    </td>
  </tr>
  <tr>
    <td><b>🏷️ Classes</b></td>
    <td>
      <img src="https://img.shields.io/badge/knife-0d1117?style=flat-square&color=E74C3C&labelColor=0d1117" />
      <img src="https://img.shields.io/badge/long_gun-0d1117?style=flat-square&color=8E44AD&labelColor=0d1117" />
      <img src="https://img.shields.io/badge/no_weapon-0d1117?style=flat-square&color=95A5A6&labelColor=0d1117" />
      <img src="https://img.shields.io/badge/pistol-0d1117?style=flat-square&color=F1C40F&labelColor=0d1117" />
    </td>
  </tr>
  <tr>
    <td><b>🧰 Format</b></td>
    <td>YOLO: <code>class x_center y_center width height</code> (normalized)</td>
  </tr>
  <tr>
    <td><b>📜 License</b></td>
    <td>
      <img src="https://img.shields.io/badge/MIT-0d1117?style=flat-square&color=CFCFCF&labelColor=0d1117" />
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

## 🧪 Split Mix

<p>
  <img src="https://img.shields.io/badge/Train-82.76%25-0d1117?style=flat-square&color=6BA7FF&labelColor=0d1117" />
  <img src="https://img.shields.io/badge/Valid-12.73%25-0d1117?style=flat-square&color=B085F5&labelColor=0d1117" />
  <img src="https://img.shields.io/badge/Test-4.51%25-0d1117?style=flat-square&color=40C4C4&labelColor=0d1117" />
</p>

<pre>
Train  [███████████████████████████████████████░░] 82.76% (49,079)
Valid  [██████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░] 12.73% (7,552)
Test   [███░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░]  4.51% (2,674)
</pre>

---

## 🎯 Class Mix (All Splits)

<p>
  <img src="https://img.shields.io/badge/KNIFE-13,010_(16.96%25)-E74C3C?style=for-the-badge&labelColor=2A0F0F" />
  <img src="https://img.shields.io/badge/LONG_GUN-22,964_(29.94%25)-8E44AD?style=for-the-badge&labelColor=1E0F2A" />
  <img src="https://img.shields.io/badge/NO_WEAPON-12,141_(15.83%25)-95A5A6?style=for-the-badge&labelColor=1B1F24" />
  <img src="https://img.shields.io/badge/PISTOL-28,590_(37.27%25)-F1C40F?style=for-the-badge&labelColor=2A250F" />
</p>

> Class distribution chart: `./assets/class_distribution.png`  
> (Copy from `/home/constantin/Doctorat/YoloLib/Utils/Scripts/merged_dataset/class_distribution.png` into `./assets/`.)

---

## 🗂️ Structure & Labels

- **Annotation format:** `class_id x_center y_center width height` (all normalized to `[0,1]`)
- **Index map:**
