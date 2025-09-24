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




## 📈 Model Comparison — Small-Object-Optimized YOLO vs Baseline

### 🎯 Why we built and compared these models

Real deployments are unforgiving: weapons often appear **tiny** (distance), **partially occluded**, and under **low-light / motion blur**. Our baseline models missed many such cases, while “look-alikes” (phones, tools, hands, reflections) inflated false positives. We therefore built a **small-object-optimized** variant to raise tiny-object recall without sacrificing practical latency.  
**Observed benefits:** more hits on distant/occluded weapons, better tolerance in noisy frames, and fewer spurious alerts after modest threshold tuning—with only a modest compute/VRAM increase from an extra detection head (P2).  

---

### A) What changed (at a glance)

| Aspect | Small-Object Optimized (ours) | Baseline | Why it helps / Notes |
|---|---|---|---|
| **Detector heads** | **P2–P5 (4 heads)** incl. **P2 @ 1/4 stride** | P3–P5 (3 heads) | Higher-res grid improves coverage for very small boxes; expect more boxes for NMS and a small latency/VRAM increase. :contentReference[oaicite:0]{index=0} |
| **P2 pathway** | Upsample + concat with early features (e.g., C3k2), **~256-ch** blocks | — | Preserves fine texture lost at downsampling; gives the head extra capacity for minute cues. :contentReference[oaicite:1]{index=1} |
| **Post-processing** | NMS IoU **≈ 0.50–0.55**, confidence **+0.02** vs baseline | Default | Curbs false positives in dense/cluttered scenes; tune per dataset. :contentReference[oaicite:2]{index=2} |
| **Where it shines** | Small, dense, crowded data; tiny GT | Medium/large objects | Denser supervision at small strides → higher AP on small objects; watch FP rise in clutter and adjust thresholds. :contentReference[oaicite:3]{index=3} |

---

### B) Losses & Training (how we trained it)

- **Assigner (TaskAligned):** raise positives for tiny GT → **top-k ≈ 24–25, β ≈ 4–5**. If FPs creep up, reduce top-k or raise β slightly. :contentReference[oaicite:4]{index=4}  
- **Size-aware box weighting:** blend **inverse-area** with score; **α anneals** over epochs (prioritize tiny boxes early, balance later). Normalize weights. :contentReference[oaicite:5]{index=5}  
- **Aux center loss (small-only):** light **L1(center)** with a decaying weight to speed alignment when W×H is just a few px. :contentReference[oaicite:6]{index=6}  
- **Stability:** epoch-scheduled **clipping** for IoU/DFL; consider **grad-norm clip ≈ 5.0**. Keep DFL **reg_max** consistent with the head. :contentReference[oaicite:7]{index=7}  
- **CLS loss:** BCE (default). If imbalance persists, try **Focal(γ≈1.5, α≈0.25)**. Define “smallness” per anchor: **(24 / stride)²**. :contentReference[oaicite:8]{index=8}  
- **Augment & schedule:** random scale **~0.5–1.8**, keep mosaic but monitor label noise; slightly longer warmup; **cosine LR** with lower final LR. :contentReference[oaicite:9]{index=9}  

---

### C) Practical knobs that worked

- **Assigner:** start **top-k=24**, **β=5.0** if FPs rise.  
- **NMS/Conf:** **IoU 0.50–0.55**, **conf +0.02** vs baseline (curbs clutter FPs).  
- **Center-L1 weight:** **0.03 → 0.01** over the first ~35 epochs.  
- **Aug scale:** **0.5–1.8**; keep mosaic if labels are clean.  
- **Eval:** always report **AP on small objects** separately; track **FP vs object area**. :contentReference[oaicite:10]{index=10}  

---

<details>
  <summary><b>🔧 Reproduce (pseudo-config)</b> — click to expand</summary>

```yaml
# Detector
detect_heads: [P2, P3, P4, P5]         # add P2 @ stride 4
p2_width_channels: 256                  # richer features around P2

# Assigner (TaskAligned)
assigner:
  name: TaskAligned
  topk: 24
  beta: 5.0

# Box loss weighting
box_loss:
  scheme: inverse_area_blend            # blend(score, 1/area)
  alpha_anneal: true                    # prioritize tiny boxes early

# Auxiliary center loss for small GT
center_aux:
  enable_small_only: true
  weight_schedule: [0.03, 0.01, 35]     # start, end, epochs
  smallness_threshold: "(24/stride)^2"  # per-anchor definition

# Stability
stability:
  iou_clip_schedule: true
  dfl_clip_schedule: true
  grad_norm_clip: 5.0
  dfl:
    reg_max: 16                         # keep consistent with head

# Classification loss
cls_loss:
  type: BCE                             # or Focal: {gamma: 1.5, alpha: 0.25}

# Post-processing
nms:
  iou: 0.52
  conf_offset: +0.02

# Augment & schedule
augment:
  random_scale: [0.5, 1.8]
  mosaic: true
scheduler:
  type: cosine
  final_lr_factor: 0.1                  # lower final LR
  warmup: longer

