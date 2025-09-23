<!-- Optional banner (replace with your own image in ./assets/) -->
<p align="center">
  <img src="./assets/hero_banner.png" alt="NewWeaponDataset" width="85%">
</p>

<h1 align="center">🔫🗡️ <span>NewWeaponDataset</span></h1>
<p align="center">
  <em>Multi-class object detection dataset for weapons & background negatives — tuned for small objects, surveillance, and cluttered scenes.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Format-YOLOv5%2Fv8-1f77b4?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-6c757d?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Images-59.3k-2ca02c?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Instances-76.7k-d62728?style=for-the-badge" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Train-82.76%25-228be6?style=flat-square" />
  <img src="https://img.shields.io/badge/Valid-12.73%25-845ef7?style=flat-square" />
  <img src="https://img.shields.io/badge/Test-4.51%25-15aabf?style=flat-square" />
</p>

---

## 🎯 Classes (with color chips)

<p>
  <img src="https://img.shields.io/badge/knife-13,010-e74c3c?style=for-the-badge" />
  <img src="https://img.shields.io/badge/long_gun-22,964-8e44ad?style=for-the-badge" />
  <img src="https://img.shields.io/badge/no_weapon-12,141-95a5a6?style=for-the-badge" />
  <img src="https://img.shields.io/badge/pistol-28,590-f1c40f?style=for-the-badge" />
</p>

> **Totals:** 76,705 instances across **59,305** images.  
> **Class distribution chart:** `./assets/class_distribution.png`  
> (Current local path: `/home/constantin/Doctorat/YoloLib/Utils/Scripts/merged_dataset/class_distribution.png` — copy it into `./assets/` to display above.)

---

## 📦 Dataset Snapshot

- **Images:** 59,305  
- **Instances:** 76,705  
- **Null/empty labels:** 0  
- **Split mix:**



<details>
<summary><b>🔎 Per-split counts</b></summary>

**Train (49,079 images)**  
- knife: 10,511 • long_gun: 19,273 • no_weapon: 10,161 • pistol: 23,507

**Valid (7,552 images)**  
- knife: 1,813 • long_gun: 2,750 • no_weapon: 1,324 • pistol: 3,843

**Test (2,674 images)**  
- knife: 686 • long_gun: 941 • no_weapon: 656 • pistol: 1,240
</details>

---

## 🗂️ Structure & Format

- **Annotation format (YOLO):**  
`class_id x_center y_center width height` (normalized to [0, 1])

- **Class index map:**

