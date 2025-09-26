<!-- Optional banner -->

<p align="center">
  <img src="https://github.com/user-attachments/assets/0754c712-7237-44ff-b93b-e7b061b34bcd" alt="test1gun" width="30%">
  <img src="https://github.com/user-attachments/assets/07c743cf-aff7-4231-9f3a-88f1612b5ee9" alt="test2gun" width="30%">
  <img src="https://github.com/user-attachments/assets/919c529b-797b-4124-9ffd-931b765fd53a" alt="test3gun" width="30%">
</p>

<h1 align="center">🔫🗡️ NewWeaponDataset</h1>
<div align="left" style="font-family: ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Roboto, Ubuntu, Cantarell, 'Noto Sans', 'Helvetica Neue', Arial; font-size: 15px; line-height: 1.6;">
  <h3 style="margin:0 0 8px 0;">🧩 Small-Object Weapon Detection Dataset</h3>
  <p>
    Public, small-object-focused dataset for multi-class weapon detection covering
    <b>knife</b>, <b>pistol</b>, <b>long_gun</b>, and a <b>no_weapon</b> hard-negative class.
    Sourced from <b>≈1,200 YouTube videos</b> 🎥; representative frames were extracted to capture a wide variety of
    <b>resolutions</b>, <b>aspect ratios</b>, and <b>scene types</b> (🌞 day / 🌙 night, CCTV and handheld).
    Scenes include <b>occlusions</b>, <b>motion blur</b>, and <b>cluttered backgrounds</b> to stress-test tiny targets 🔎.
  </p>

  <p>
    <b>Why <code>no_weapon</code>?</b> 🚫🔫
    Explicit negatives teach the model to distinguish real weapons from visually similar items
    (phones, tools, umbrellas, camera rigs), which <b>reduces false positives</b> and improves precision
    in crowded or low-quality footage.
  </p>




</div>


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

### 🧪 Split Mix

<p align="left" style="margin:0;">
  <img src="https://img.shields.io/badge/Train-82.76%25-228be6?style=flat-square&labelColor=111827" alt="Train 82.76%" style="margin:2px 6px 2px 0;" />
  <img src="https://img.shields.io/badge/Valid-12.73%25-845ef7?style=flat-square&labelColor=111827" alt="Valid 12.73%" style="margin:2px 6px 2px 0;" />
  <img src="https://img.shields.io/badge/Test-4.51%25-15aabf?style=flat-square&labelColor=111827" alt="Test 4.51%" style="margin:2px 6px 2px 0;" />
</p>

<pre>
Train  [███████████████████████████████████████░░] 82.76% (49,079)
Valid  [██████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░] 12.73% (7,552)
Test   [███░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░]  4.51% (2,674)
</pre>

### 📊 Class Distribution
<p align="left" style="margin:0;">
  <img src="https://img.shields.io/badge/knife-13,010_(16.96%25)-A61E4D?style=flat-square&labelColor=111827" alt="knife: 13,010 (16.96%)" />
  <img src="https://img.shields.io/badge/long_gun-22,964_(29.94%25)-7C3AED?style=flat-square&labelColor=111827" alt="long_gun: 22,964 (29.94%)" />
  <img src="https://img.shields.io/badge/no_weapon-12,141_(15.83%25)-6B7280?style=flat-square&labelColor=111827" alt="no_weapon: 12,141 (15.83%)" />
  <img src="https://img.shields.io/badge/pistol-28,590_(37.27%25)-D97706?style=flat-square&labelColor=111827" alt="pistol: 28,590 (37.27%)" />
</p>


### 📊 Dataset Examples

<table>
  <tr>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/af5b7f23-f809-404d-8da0-17ddc436f894" alt="Example 1" width="100%" />
      <br><sub>Example 1</sub>
    </td>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/b0805ccc-09e6-4167-abcb-35a583532762" alt="Example 2" width="100%" />
      <br><sub>Example 2</sub>
    </td>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/dbab2e81-8b7b-45b4-be47-50eb64689d9d" alt="Example 3" width="100%" />
      <br><sub>Example 3</sub>
    </td>
  </tr>
</table>




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


<div align="center">

## 🔎 YOLOv12s — Small-Object Focused Variant (P2–P5 + loss tweaks)

<sub><em>A compact introduction to what changed, why we changed it, and how it helps tiny objects.</em></sub>

</div>

> **Why this exists**  
> Small objects often disappear at standard detection strides (P3–P5). We introduce a P2–P5 head and loss-function tweaks to increase supervision and signal quality on tiny targets—without derailing your existing YOLOv12s workflow.

---

## ✨ What we compared

- **Baseline:** original **YOLOv12s** with a **P3–P5** detection head and **Ultralytics default loss**.  
- **Custom:** **YOLOv12s (P2–P5)** with architectural upgrades **+ small-object-aware loss**.

---

## 🧠 Key architectural changes (P2–P5 head vs standard P3–P5)

- Add a **P2 head (stride 1/4)** so tiny objects are observed at higher spatial resolution.
- **Strengthen the P2 branch** with **256-channel Conv/A2C2f** blocks to keep fine detail.
- Use **four detection heads (P2, P3, P4, P5)** instead of three (**P3–P5**).
- **Slightly adjust post-processing:** consider **lower NMS IoU** for dense tiny objects.


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


## 🔧 Loss: Modified vs Ultralytics Baseline

- **Assigner (TaskAligned)** — `topk=25`, `beta=4.0` (baseline `topk=10`, `beta=6.0`).  
  *Why:* increases positives and softens the gate → higher recall on tiny boxes.  
  *Tip:* if FPs rise, try `topk=20–24`, `beta≈5`.

- **Size-aware box weighting** — blend inverse area and classification score:  
  `w = α·(1/area) + (1−α)·score`, with **α annealed** over epochs.  
  *Why:* emphasizes very small boxes early, then balances with score later.  
  *Tip:* normalize weights; `sqrt(area)` can improve stability.

- **Auxiliary center L1** — applied **only to small GT** with a **decaying weight**.  
  *Why:* speeds up center alignment when `W×H` is just a few pixels.  
  *Tip:* compute “smallness” **per-anchor stride**.

- **Epoch-scheduled clipping (IoU/DFL)**.  
  *Why:* reduces loss spikes/instability in dense tiny-object scenes.  
  *Tip:* optional grad-norm clip (e.g., `5.0`).

- **Detection classification (CLS)** — keep **BCE** by default; switch to **Focal** if class imbalance persists.  
  *Tip:* start with **Focal** `γ≈1.5`, `α≈0.25` if small-class recall is low.

- **OBB classification** — use **Focal**.  
  *Why:* more robust to class imbalance.  
  *Cost:* slightly slower; tune `γ/α` as needed.



### 📦 Loss & Assigner Tweaks (tiny-object oriented)

| Aspect                | Modified (yours)                                       | Baseline           | Effect on tiny objs                                      | Trade-offs / tips                                                                 |
|-----------------------|--------------------------------------------------------|--------------------|----------------------------------------------------------|-----------------------------------------------------------------------------------|
| Assigner top-k / β    | `topk=25, β=4.0`                                       | `topk=10, β=6.0`   | More positives & softer gate → higher recall             | May add noisy positives; try `topk=20–24`, `β≈5` if FPs rise                      |
| Box weighting         | Inverse-area × (α) + score × (1-α), α anneals          | Score-only         | Prioritizes small boxes early, balances later            | Normalize weights; consider `sqrt(area)` for stability                            |
| Center aux loss       | L1 on centers for small GT (decay)                     | —                  | Faster center alignment when `W×H` is a few px           | Compute smallness per-anchor stride                                               |
| Loss clipping         | Epoch-scheduled caps for IoU/DFL                       | —                  | Tames spikes in tiny crowded scenes                      | Also consider grad-norm clip (e.g., `5.0`)                                        |
| DFL details           | Size-aware weighting                                   | Standard DFL       | Stabilizes edge bins for small boxes                     | Keep `reg_max` consistent with head                                               |
| CLS loss (detect)     | BCE (unchanged; option: **Focal**)                     | BCE                | —                                                        | Use Focal (`γ≳1.5`, `α≈0.25`) if small-class recall is low                        |
| CLS loss (OBB)        | **Focal**                                              | BCE                | Better imbalance handling                                | Slightly slower; tune `γ/α`                                                       |
| Smallness threshold   | `(24 / stride)^2` (per-anchor)                          | —                  | Targets truly tiny instances                             | Use **per-anchor** threshold; avoid relying only on a global min stride           |


## 📊 Comparison Results

### 1) Detection Confidence Interval Stats

| Confidence Interval | Original: Count (Avg Conf) | Custom: Count (Avg Conf) | Winner / Note                         |
| --- | --- | --- | --- |
| 0.5–0.6 | 0 (0.000) | 0 (0.000) | Tie |
| 0.6–0.7 | 600 (0.654) | 480 (0.658) | Original |
| 0.7–0.8 | 1128 (0.755) | 1155 (0.757) | Custom |
| 0.8–0.9 | 676 (0.828) | 1243 (0.842) | Custom (more high-conf hits) |
| 0.9–1.0 | 0 (0.000) | 26 (0.908) | Custom (more high-conf hits) |

---

### 2) Per-Class Detection Statistics

| Class     | Original: Detections (Avg Conf) | Custom: Detections (Avg Conf) | Winner |
| --- | --- | --- | --- |
| Knife     | 525 (0.746) | 593 (0.786)  | Custom |
| Long Gun  | 698 (0.746) | 814 (0.781)  | Custom |
| No Weapon | 245 (0.731) | 386 (0.740)  | Custom |
| Pistol    | 936 (0.761) | 1111 (0.787) | Custom |

## 3) Detection Accuracy per Class (TP/FP/FN, P/R, F1)

| Class     | Original TP/FP/FN | Original P/R | Original F1 | Custom TP/FP/FN | Custom P/R | Custom F1 | Winner (F1) |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Knife     | 487/38/199  | 0.93 / 0.71 | 0.805 | 539/54/147  | 0.91 / 0.79 | 0.846 | Custom |
| Long Gun  | 648/50/293  | 0.93 / 0.69 | 0.792 | 745/69/196  | 0.92 / 0.79 | 0.850 | Custom |
| No Weapon | 207/38/449  | 0.84 / 0.32 | 0.463 | 302/84/354  | 0.78 / 0.46 | 0.579 | Custom |
| Pistol    | 882/54/358  | 0.94 / 0.71 | 0.809 | 1020/91/220 | 0.92 / 0.82 | 0.867 | Custom |

---

## 4) Overall Metrics

| Metric                         | Original | Custom |
| --- | --- | --- |
| Precision                      | 0.9251  | 0.8974 |
| Recall                         | 0.6313  | 0.7397 |
| F1 (from overall P/R)          | 0.750   | 0.811  |
| False Positives (FPs)          | 180     | 298    |
| False Negatives (FNs)          | 1299    | 917    |
| False Positive Rate            | 7.49%   | 10.26% |
| Avg FP Confidence              | 0.7075  | 0.7145 |
| Total Predictions > threshold  | 2404    | 2904   |
| Average Prediction Confidence  | 0.7503  | 0.7787 |


## ✅ Conclusion

**TL;DR:** The custom **YOLOv12s (P2–P5 + loss tweaks)** delivers **meaningfully higher recall and F1**—especially on small, crowded targets—at the cost of a modest **precision** drop due to more FPs.

### What the numbers say
- **Confidence shift to higher bands:** more hits in **0.8–0.9** and even **0.9–1.0** vs. baseline.
- **Per-class gains across the board:** F1 improves for **Knife, Long Gun, No Weapon, Pistol** (largest jump on *No Weapon*).
- **Overall metrics:**
  - **Recall:** **0.631 → 0.740** (↑ ~11 pts), **FNs:** **1299 → 917** (−382).
  - **F1:** **0.750 → 0.811** (↑ ~6 pts).
  - **Precision:** **0.925 → 0.897** (↓ ~2.8 pts), **FPs:** **180 → 298** (↑ 118).


<h4>🔍 Detection Examples</h4>

<table>
<tr>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/89bc6fd9-a52f-4620-8611-9f63bd392599" alt="7_compare" width="100%"><br><sub>7_compare</sub></td>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/c50d8762-7e5f-40c3-9e4e-ad8754f5a5dd" alt="13_compare" width="100%"><br><sub>13_compare</sub></td>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/d7f883cb-bb85-4432-ad97-285c2e27ddb8" alt="36_compare" width="100%"><br><sub>36_compare</sub></td>
</tr>

<tr>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/e2167e20-c0a4-4f4b-8bf9-a8ad4ec9c6fb" alt="68_compare" width="100%"><br><sub>68_compare</sub></td>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/a215bab3-9899-4ae2-a6e6-cb5a4e9641a3" alt="127_compare" width="100%"><br><sub>127_compare</sub></td>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/cb07b5fc-f636-4d43-b737-d0ea129045cd" alt="128_compare" width="100%"><br><sub>128_compare</sub></td>
</tr>

<tr>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/24eb0e7d-72d3-4af7-b3fd-9597424a804d" alt="132_compare" width="100%"><br><sub>132_compare</sub></td>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/29c1e79b-d06c-427b-b96e-e531b64c3282" alt="151_compare" width="100%"><br><sub>151_compare</sub></td>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/743218e8-fbd7-4b1b-8574-8a68bdc7baa1" alt="200_compare" width="100%"><br><sub>200_compare</sub></td>
</tr>

<tr>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/bdfe84c2-a815-48e9-b0d2-a95208ac5505" alt="306_compare" width="100%"><br><sub>306_compare</sub></td>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/1c40f69d-78a6-4aed-8cdc-4fa1cf0ba8a9" alt="560_compare" width="100%"><br><sub>560_compare</sub></td>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/3b4a5d00-ce5a-49e9-a2d1-8b4b54790740" alt="873_compare" width="100%"><br><sub>873_compare</sub></td>
</tr>

<tr>
<td align="center" width="33%"><img src="https://github.com/user-attachments/assets/bc057716-be5d-42fa-a9a5-addd65926797" alt="1894_compare" width="100%"><br><sub>1894_compare</sub></td>
<td width="33%"></td>
<td width="33%"></td>
</tr>
</table>


<h4>📈 Model Comparison — Confusion & Training</h4>

<table>
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/09326857-5418-4a62-836e-f9ec443327ff" alt="confusion_matrix_custom_model" width="100%" />
      <br><sub>Confusion Matrix — Custom Model</sub>
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/6faf2f7b-6679-4270-a389-0ac0c3e96a78" alt="confusion_matrix_original_model" width="100%" />
      <br><sub>Confusion Matrix — Original Model</sub>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/74b5d9eb-638f-4360-a07d-d66cab2dfbbb" alt="training_results_custom_model" width="100%" />
      <br><sub>Training Results — Custom Model</sub>
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/d064675b-c23a-4aea-a71a-dfcadb355f8f" alt="training_results_original_model" width="100%" />
      <br><sub>Training Results — Original Model</sub>
    </td>
  </tr>
</table>


<!-- ===================== Model Comparison ===================== -->
<div align="left" style="font-family: ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Roboto, Ubuntu, Cantarell, 'Noto Sans', 'Helvetica Neue', Arial; line-height:1.6; font-size:15px;">

  <h3 style="margin:0 0 10px 0;">📈 Model Comparison — Custom vs Original</h3>

  <p style="margin:0 0 12px 0;">
    Side-by-side evaluation of the <b>custom</b> vs <b>original</b> model using normalized confusion matrices and training curves.
    The custom model targets small objects and hard negatives (<code>no_weapon</code>).
  </p>

  <h4 style="margin:14px 0 6px 0;">🔢 Confusion Matrices (Normalized)</h4>
  <ul style="margin:0 0 10px 18px;">
    <li><b>Knife</b>: <b>0.88</b> (custom) vs 0.87 (orig) — <span title="+0.01">small gain</span>.</li>
    <li><b>Long_gun</b>: <b>0.89</b> vs 0.86 — clear gain <b>(+0.03)</b>.</li>
    <li><b>Pistol</b>: <b>0.91</b> vs 0.89 — clear gain <b>(+0.02)</b>.</li>
    <li><b>no_weapon</b>: <b>0.61</b> vs 0.53 — biggest improvement <b>(+0.08)</b>, better separation from weapon classes.</li>
  </ul>
  <p style="margin:0 0 12px 0;">
    <i>Note:</i> Both models still show some spill into <b>background</b> (≈0.24–0.29 off-diagonal), which is the main remaining error bucket.
  </p>

  <h4 style="margin:14px 0 6px 0;">📉 Training Curves</h4>
  <ul style="margin:0 0 10px 18px;">
    <li><b>Losses (train/val box, cls, dfl)</b>: custom converges lower and more smoothly after ~epoch 10.</li>
    <li><b>Precision</b>: both plateau around <b>≈0.86</b>; custom is slightly steadier.</li>
    <li><b>Recall</b>: both around <b>≈0.75–0.77</b>; custom edges higher and holds late-epoch stability.</li>
    <li><b>mAP@50 / mAP@50–95</b>: on par or <b>~+1–2 pts</b> for the custom run.</li>
  </ul>

  <div style="margin:12px 0; padding:10px 12px; border:1px solid #e5e7eb; border-radius:8px;">
    <b>TL;DR</b> — The <b>custom model</b> is consistently stronger on all weapon classes and
    <b>notably better</b> at identifying <code>no_weapon</code>, while keeping precision/recall at least as good and driving losses lower.
    Remaining work: reduce background confusions.
  </div>

  <h4 style="margin:14px 0 6px 0;">🛠️ Next Steps</h4>
  <ul style="margin:0 0 0 18px;">
    <li>Expand/upsample <b>hard negatives</b> (crowds, hands, tools, phones) to push down background/no_weapon mix-ups.</li>
    <li>Tune <b>class-wise confidence &amp; NMS</b> (slightly higher for pistol/long_gun, slightly lower for no_weapon).</li>
    <li>Try <b>class-balanced sampling</b> and a short <b>low-LR fine-tune</b> on the latest data mix.</li>
  </ul>

</div>
<!-- ============================================================ -->



