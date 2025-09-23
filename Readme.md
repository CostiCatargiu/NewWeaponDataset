<!-- Optional banner (replace with your own image in ./assets/) -->
<p align="center">
  <img src="./assets/hero_banner.png" alt="NewWeaponDataset" width="85%">
</p>

<h1 align="center">🔫🗡️ <span>NewWeaponDataset</span></h1>
<p align="center">
  <em>A high-quality, small-object-focused dataset for multi-class weapon detection (knife, pistol, long_gun) and hard negatives (no_weapon), curated from diverse day/night CCTV and handheld scenes with occlusions and clutter. Designed for robust surveillance models and research on tiny targets.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Format-YOLOv5%2Fv8-1f77b4?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-6c757d?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Hosted-Roboflow%20Universe-20c997?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Public-Yes-2ca02c?style=for-the-badge" />
</p>

> **Availability:** Public on **Roboflow Universe** — add your link here: **`<INSERT_ROBOFLOW_UNIVERSE_LINK>`**

---

## 📦 Dataset Snapshot

| Key                  | Value                              |
|----------------------|------------------------------------|
| Images               | **59,305**                         |
| Instances            | **76,705**                         |
| Null/empty labels    | **0**                              |
| Classes              | `knife`, `long_gun`, `no_weapon`, `pistol` |
| Format               | YOLO (`class x_center y_center width height`, normalized) |
| License              | MIT                                |
| Focus                | Small objects, occlusion, motion blur, varied lighting |
| Hosting              | Roboflow Universe (public)         |

---

## 🔀 Split Mix

| Split | Images | % of total |
|------:|-------:|-----------:|
| Train | 49,079 | **82.76%** |
| Valid | 7,552  | **12.73%** |
| Test  | 2,674  | **4.51%**  |
| **Total** | **59,305** | **100%** |

---

## 🏷️ Class Totals (All Splits)

| Class      | Instances | Share |
|------------|----------:|------:|
| knife      | 13,010    | 16.96% |
| long_gun   | 22,964    | 29.94% |
| no_weapon  | 12,141    | 15.83% |
| pistol     | 28,590    | 37.27% |
| **Total**  | **76,705**| **100%** |

---

## 📊 Per-Split Class Counts

| Class     | Train  | Valid | Test | **Total** |
|-----------|-------:|------:|-----:|----------:|
| knife     | 10,511 | 1,813 | 686  | **13,010** |
| long_gun  | 19,273 | 2,750 | 941  | **22,964** |
| no_weapon | 10,161 | 1,324 | 656  | **12,141** |
| pistol    | 23,507 | 3,843 | 1,240| **28,590** |

---

## 🗂️ Class Index Map

| Index | Class     |
|------:|-----------|
| 0     | knife     |
| 1     | long_gun  |
| 2     | no_weapon |
| 3     | pistol    |

> **Annotation format (YOLO):** `class_id x_center y_center width height` (all values normalized to `[0,1]`).

---

## 🧪 Tips

- For tiny targets, consider larger `imgsz` (e.g., 960–1280), tuned augmentations, and careful NMS thresholds.
- Include `no_weapon` in validation metrics to track false positives in cluttered backgrounds.

---

## 📈 Visuals

- Class distribution chart: `./assets/class_distribution.png`  
  _(Copy from your local path `/home/constantin/Doctorat/YoloLib/Utils/Scripts/merged_dataset/class_distribution.png` into `./assets/` to render here.)_

---

## 🚀 Quick Start (YOLOv8)

```bash
pip install ultralytics
yolo task=detect mode=train model=yolov8n.pt data=data.yaml epochs=50 imgsz=640
