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
    <img src="https://img.shields.io/badge/Open%20NoGun%20Dataset-000?logo=roboflow&logoColor=white&style=for-the-badge" alt="Open NoGun Dataset on Roboflow">
  </a>
  <a href="https://app.roboflow.com/gundetectiondataset/weapondataset-oi2g3/8">
    <img src="https://img.shields.io/badge/Open%20WeaponDataset%20v8-000?logo=roboflow&logoColor=white&style=for-the-badge" alt="Open WeaponDataset v8 on Roboflow">
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
    <td>
      <a href="https://universe.roboflow.com/gundetectiondataset/nogun/dataset/2">Roboflow Universe: NoGun</a> &nbsp;•&nbsp;
      <a href="https://app.roboflow.com/gundetectiondataset/weapondataset-oi2g3/8">Roboflow App: WeaponDataset v8</a>
    </td>
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

<details>
  <summary>📷 Dataset examples — click to expand</summary>

  <table>
    <tr>
      <td align="center">
        <img src="https://github.com/user-attachments/assets/af5b7f23-f809-404d-8da0-17ddc436f894" alt="Example 1" width="100%" />
        <br><sub>Example 1</sub>
      </td>
      <td align="center">
        <img src="https://github.com/user-attachments/assets/b0805ccc-09e6-4167-abcb-35a583532762" alt="Example 2" width="100%" />
        <br><sub>Example 2</sub>
      </td>
      <td align="center">
        <img src="https://github.com/user-attachments/assets/dbab2e81-8b7b-45b4-be47-50eb64689d9d" alt="Example 3" width="100%" />
        <br><sub>Example 3</sub>
      </td>
    </tr>
  </table>
</details>



<details>
  <summary>📊 Class distribution chart - click to expand </summary>

  <p align="center">
    <img src="https://github.com/user-attachments/assets/5b18d380-a33e-47e3-aadd-eb3769f93447"
         alt="class_distribution" width="100%">
  </p>
</details>

<details>
  <summary>📊 Training Setup - click to expand </summary>

  <p align="center">
    <img src="https://github.com/user-attachments/assets/ef61fcfc-5545-40ef-881b-d1cb6b2fcb23"
         alt="class_distribution" width="100%">
  </p>
</details>


---

## 🗂️ Structure & Labels

- **Annotation format:** `class_id x_center y_center width height` (all normalized to `[0,1]`)
- **Index map:**


<div align="center">

# 🔎 YOLOv12s — Small-Object Focused Variant (P2–P5 + loss tweaks)

<sub><em>A compact introduction to what changed, why we changed it, and how it helps tiny objects.</em></sub>

</div>

> **Why this exists**  
> Small objects often disappear at standard detection strides (P3–P5). We introduce a P2–P5 head and loss-function tweaks to increase supervision and signal quality on tiny targets—without derailing your existing YOLOv12s workflow.

---

## ✨ What we compared

- **Baseline:** original **YOLOv12s** with a **P3–P5** detection head and **Ultralytics default loss**.  
- **Custom:** **YOLOv12s (P2–P5)** with architectural upgrades **+ small-object-aware loss**.

---

## 🧠 Key architectural changes (P2–P5)

- **Add P2 head (stride 1/4):** exposes tiny objects to higher spatial resolution.
- **Strengthen P2 branch:** **256-channel Conv/A2C2f** blocks to preserve fine texture/edges.
- **Four heads instead of three:** **P2, P3, P4, P5** (vs. baseline P3–P5) for better scale specialization.
- **Post-processing nudge:** in dense tiny-object scenes, consider a **lower NMS IoU**.

---

## 📉 Loss-function intent (small-object aware)

- **Classification:** quality-aware weighting so small positives aren’t drowned out by easy negatives.  
- **Box regression:** **area-aware emphasis** to keep tiny boxes from being underfit.

---

## 🔬 Baseline vs Custom (at a glance)

| Aspect | Baseline YOLOv12s | Custom YOLOv12s (this work) |
| --- | --- | --- |
| Detect heads | **P3–P5** | **P2–P5** |
| Tiny-object exposure | Limited (stride ≥ 1/8) | **High** (adds stride **1/4** grid) |
| P2 branch capacity | — | **256-ch Conv/A2C2f** for fine detail |
| Loss focus | Ultralytics default | **Small-object-aware** (quality + area cues) |
| NMS guidance | Default | **Lower IoU** recommended in dense scenes |

---

## ⚙️ Practical knobs

- **NMS IoU:** try **0.50–0.55** when tiny instances cluster densely.  
- **Confidence threshold:** tune slightly **lower** if recall on small objects matters most.  
- **Augmentations:** mosaic / random scale can help tiny GT land on **P2/P3** (watch for label noise).

---

> **TL;DR**  
> We compared the original YOLOv12s to a custom P2–P5 variant and small-object-aware loss. The changes are targeted, practical, and aimed at **raising AP\_S** with modest compute overhead—especially in crowded, tiny-object datasets.



### Tiny-object settings: P2–P5 vs P3–P5 (single table)

| Aspect             | P2–P5 (yours)                            | P3–P5 (baseline)  | Why it helps / guidance                           | Trade-offs / notes                      |
| ------------------ | ---------------------------------------- | ----------------- | ------------------------------------------------- | --------------------------------------- |
| Output strides     | P2 (1/4), P3 (1/8), P4 (1/16), P5 (1/32) | P3–P5 only        | High-res P2 grid covers very small boxes          | More memory/compute; more boxes for NMS |
| P2 pathway         | Upsample + concat with early C3k2        | —                 | Preserves fine edges/texture lost at downsampling | Ensure BN/act stats are stable          |
| Head width near P2 | 256-ch Conv/A2C2f                        | Typically 192–256 | Extra capacity for minute cues                    | Slight latency/VRAM increase            |
| # Detect heads     | 4 (P2–P5)                                | 3 (P3–P5)         | More scale-specialization                         | Heavier training; tune                  |
| AP\_S (tiny)       | Usually higher                           | Lower             | Denser supervision at small strides               | Potential FP rise in clutter            |
| Best with          | Small, dense, crowded datasets           | Medium/large objects | Matches receptive field to object size         | Try lower NMS IoU 0.50–0.55            |
| Aug synergy        | Strong with mosaic & random scale ↑      | Moderate          | Upscaled tiny GT land on P2/P3                    | Watch label noise with heavy aug        |

