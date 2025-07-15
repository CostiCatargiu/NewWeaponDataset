<h1 align="center">🔫🗡️ NewWeaponDataset</h1>
<p align="center">
Multi-class object detection dataset for weapons and miscellaneous objects — optimized for security & surveillance use cases.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Format-YOLOv5/v8-green" />
  <img src="https://img.shields.io/badge/Classes-knife|pistol|longgun|other-blue" />
  <img src="https://img.shields.io/badge/License-MIT-lightgrey" />
</p>

---

## 📁 Dataset Structure


> ✅ Annotations are in YOLO format:  
> `class_id x_center y_center width height` (normalized)

---

## 🏷️ Classes

| Class   | Description                                       |
|---------|---------------------------------------------------|
| `knife` | Folding, kitchen, tactical knives                 |
| `pistol`| Handguns, revolvers, semi-automatic pistols       |
| `longgun` | Shotguns, rifles, large firearms                |
| `other` | Non-weapon items: phones, umbrellas, tools, etc.  |

---

## 🧠 Features

- 🔍 Small object detection ready
- 🌗 Day/night scenes
- 🧱 Complex backgrounds with occlusions
- 🎯 Balanced samples of weapons & non-weapons

---

## 📸 Example Images

<!-- Replace below with actual image links or use local images -->
<p align="center">
  <img src="sample1.jpg" width="45%" /> 
  <img src="sample2.jpg" width="45%" />
</p>

---

## 🚀 Use Cases

- 🔒 Real-time surveillance & public safety
- 🤖 Training custom YOLO/SSD/Faster R-CNN models
- 📊 Research on object detection under occlusion & clutter

---

## 🛠️ Training Example (YOLOv8)

```bash
yolo task=detect mode=train model=yolov8n.pt data=dataset.yaml epochs=50 imgsz=640
