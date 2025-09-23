<h1 align="center">🔫🗡️ NewWeaponDataset</h1>
<p align="center">
Multi-class object detection dataset for weapons and negatives — optimized for security & surveillance use cases.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Format-YOLOv5/v8-green" />
  <img src="https://img.shields.io/badge/Classes-knife|pistol|long_gun|no_weapon-blue" />
  <img src="https://img.shields.io/badge/License-MIT-lightgrey" />
</p>

---

## 📦 Dataset Snapshot

- **Total images:** 59,305  
- **Splits:** Train 49,079 (82.76%) • Valid 7,552 (12.73%) • Test 2,674 (4.51%)  
- **Total annotations (all splits):** 76,705 instances  
- **Null/empty label files:** 0

### 🏷️ Class Totals (All Splits)

| Class       | Instances | Share |
|-------------|-----------:|------:|
| knife       | 13,010     | 16.96% |
| long_gun    | 22,964     | 29.90% |
| no_weapon   | 12,141     | 15.83% |
| pistol      | 28,590     | 37.27% |
| **Total**   | **76,705** | 100% |

> 📊 Class distribution chart saved locally at:  
> `/home/constantin/Doctorat/YoloLib/Utils/Scripts/merged_dataset/class_distribution.png`  
> _(If you commit it, reference it here with a relative path, e.g. `./assets/class_distribution.png`.)_

---

## 📁 Split Details

**Train (49,079 images)**  
- knife: 10,511 • long_gun: 19,273 • no_weapon: 10,161 • pistol: 23,507

**Valid (7,552 images)**  
- knife: 1,813 • long_gun: 2,750 • no_weapon: 1,324 • pistol: 3,843

**Test (2,674 images)**  
- knife: 686 • long_gun: 941 • no_weapon: 656 • pistol: 1,240

---

## 🗂️ Structure & Format

- **Annotation format (YOLO):**  
  `class_id x_center y_center width height` (normalized to [0,1])

- **Classes (indices):**
  - `0: knife`
  - `1: long_gun`
  - `2: no_weapon` (negative class: scenes/objects with **no** weapon present)
  - `3: pistol`

Example `data.yaml`:
```yaml
path: <root_of_dataset>   # optional if using absolute paths below
train: <path-to-train-images>
val: <path-to-val-images>
test: <path-to-test-images>

names:
  0: knife
  1: long_gun
  2: no_weapon
  3: pistol
